###  🌱 Plant Feelings 


Plant Feelings is an interactive artwork that visualizes a plant’s emotional state using live input from a soil moisture sensor, inspired by the debate around bonsai ethics.

The plant is represented as a pixel-art character that walks, idles, follows the mouse, reacts to attention, and displays different emotional states based on real humidity levels.

This project combines:
- p5.js
- Arduino moisture sensor(capacitive soil moisture sensor())
- Pixel animation (Aseprite)
- UI/Interaction design
- A conceptual exploration of how humans empathize with plants




---

#### 🌿 Concept
This work is inspired by the ongoing debate surrounding bonsai and the ethics of shaping nature for aesthetics.
Some argue that shaping and pruning a bonsai is cruel because it forces a plant into an unnatural form.

Yet at the same time, mowing a lawn, trimming hedges, or cutting houseplants is considered normal—even though these also involve cutting and shaping plants.
This contradiction raises the central question of the project:
Why do we feel empathy toward some manipulated plants, but not others?
Plant Feelings exaggerates the idea that plants have emotions in order to highlight this inconsistency.

By giving the plant:
- A sad animation when under-watered/ignored
- A happy animation when healthy
- Physical reactions to the mouse
- Pop-up “feeling windows” representing attention or warnings

the system playfully exposes how easily humans project emotions onto non-human life.
The work invites viewers to reflect on how cultural narratives but not biology shape our perception of nature, cruelty, and empathy.

---

#### ✨ Features
- Live moisture detection using an Arduino and soil humidity sensor
- A draggable on-screen plant feeling window
- Pixel-art animations drawn and animated using **Aseprite**
- Visual mood states tied to humidity thresholds
- Interactive UI with evolving feedback

---

#### 💧 Sensor Data → Plant Emotion Mapping
The plantFeeling window expression updates based on real-time humidity levels:

| Humidity Range | Plant / feeling window State |
|----------------|------------------------------|
| ≤ 20           | Super Thirsty 😭             |
| 20–40          | Low Water 😢                 |
| 40–80          | Happy 😊                     |
| > 80           | Overwatered 😳               |
| Timer > 60s    | Needy 😔                     |

---

#### 🧩 Technical Architecture
**Hardware**
- Arduino board
- Soil moisture sensor
- Serial communication to browser

**Software**
- Penpot (for UI mockups and html/css prototyping/code)(don't look at the code its a mess thanks🙏)
- JavaScript
- p5.js (or HTML/JS canvas)
- Serial input handling
- Sprite swapping + pixel animations
- Drag interaction on mouse events

---

#### 🎨 Art & UI Workflow
All animations and sprite assets were created in **Aseprite**, requiring:
- Learning pixel animation workflows
- Designing multiple expression variations
  Th UI was created in Penpot, requiring:
- Learning Penpot for UI design
- Understanding of how penpot created code from UI prototypes to create efficient code prototyping( work smart not hard )
- Repeatedly redesigning the UI to achieve a clear, readable visual style
- Iterations to match the mood-system logic with visual pacing

These redesigns were crucial in achieving the final emotional aestetics to project clarity and polished presentation.

---

#### 🚧 Challenges
Some key challenges in the development process included:

**🎨 Learning Aseprite**
- Learning pixel art techniques from scratch
- Understanding pixel animation timing
- Creating expressive sprites with limited resolution
- Managing sprite sheets and exporting assets

**🖼 UI Redesign Iteration**
- Learning Penpot for UI prototyping from scratch
- Multiple redesign cycles to achieve the "Vibe"
- easy integration of code with UI made me indecisive and overthink design choices instead of working on the p5.js code


#### 💻 Technical Issues
- Ensuring sprite updates flowed without visual stutter
- Linking the temperature sensor with arduino leading to eventually giving up on that
- Debugging humidity thresholds and condition logic to make it cleaner
- Implementing drag mechanics without interfering with other interactions

---

#### 📈 Future Enhancements
- Additional mood states
- Sound effects matching emotion
- Growing / evolving plant character
- Save data or long-term plant “health” with a graph
- Mobile-friendly version

#### Progress shots / Videos
<image src="./documentation/Doc1Concept.png"  ></image>
<image src="./documentation/Doc2Art.png"  ></image>
<image src="./documentation/Doc3Code.png"  ></image>
<image src="./documentation/Doc4Presentation.png"  ></image>
---
#### Reflection
Creating Plant Feelings was a challenging but rewarding experience that pushed me to learn new skills in p5.js, pixel art and interactive coding. The project allowed me to explore a interesting concept around empathy for plants while honing my creative abilities. It was satisfying to see the plant character come to life with emotions tied to real sensor data, and I learned a lot about balancing art, interaction, and code. In the future, I would like to expand the project with more features and polish, but I am proud of what I accomplished within the time constraints. I look forward to working on this into the future and on my plant at home.

