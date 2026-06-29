***********************************************************************
**Tutorial:** Cognitive Architectures for Robust and Reliable Robotics
***********************************************************************
   *14:00 - 15:00 / 15:30 - 17:00* -- Esther Aguado, Carlos Hernandez Corbato

**Tutorial description:**
This practical session explores the design and implementation of a minimal hybrid cognitive architecture for autonomous robots.
Following a brief theoretical introduction — covering the role of cognitive architectures in intelligent systems, the separation-of-concerns principle, and the components of a hybrid approach — students work through three interconnected hands-on exercises.
First, they extend an OWL ontology with room and object concepts and run an OWL reasoner on live YOLO detections.
Second, they complete a belief management node that combines YOLO confidence scores with symbolic inferences, models belief strengths, and incorporates memory decay over time.
Third, they complete a goal manager node that maintains a sequence of symbolic goals and monitors the belief state to determine when each goal has been achieved.
The implementation is then validated against adversarial scenarios: visiting the wrong room first, handling ambiguous transitions, and revisiting previously explored rooms.

**Session materials:**
 - :GitHub:`estherag/intro_cognitive_architectures`

**Bio. Esther Aguado** holds a PhD in Automation and Robotics from the Polytechnic University of Madrid (UPM, 2024). Her research focuses on techniques that provide guarantees on robot behavior through introspection and adaptation.

She graduated in Industrial Technology Engineering (UPM, 2017), with a specialization in Electronics and Automation. She completed her training with a Master's degree in Industrial Engineering (UPM, 2019) and a Master's degree in Automation and Robotics (UPM, 2020). In 2019, she joined the Center for Automation and Robotics (CAR-CSIC) with a Collaboration Grant, participating in the development of sound localization systems for robots. During her PhD, she worked on the design of robust systems applied to underground mining, social robotics, and industrial robotics, with competitive predoctoral funding.

Her thesis, "SysSelf: Systems that know what they are doing," awarded Outstanding Cum Laude with International Mention, establishes a framework for autonomous systems to regulate their own control processes in real time.

She has published in JCR journals, participated in national and international conferences, and is a co-inventor of a patent. She was a visiting researcher at TU Delft (Netherlands) in 2022 and 2024. She is currently an Assistant Professor at the Rey Juan Carlos University, where she teaches Telematics Engineering and Robotics, and continues her research work on intelligent systems with behavioral guarantees.
