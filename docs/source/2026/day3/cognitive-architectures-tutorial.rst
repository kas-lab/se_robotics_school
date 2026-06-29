**************************************************************
Cognitive Architectures for Robust and Reliable Robotics
**************************************************************
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
