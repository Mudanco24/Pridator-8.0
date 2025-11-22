import random

class AvitaPredator:
    def __init__(self):
        self.position = 0
        self.direction = random.choice(['forward', 'backward'])

    def move(self):
        if self.direction == 'forward':
            self.position += 1
        else:
            self.position -= 1

        # Randomly change direction
        if random.random() < 0.2:
            self.direction = 'backward' if self.direction == 'forward' else 'forward'

    def predict_stop(self):
        # Simple prediction model
        if self.direction == 'forward':
            return self.position + random.randint(1, 3)
        else:
            return self.position - random.randint(1, 3)

# Create an Avita Predator object
predator = AvitaPredator()

# Simulate movement
for i in range(10):
    predator.move()
    print(f"Time {i+1}: Position {predator.position}, Direction {predator.direction}")
    print(f"Predicted stop: {predator.predict_stop()}")# Pridator-8.0
It has to predict the aviator 
It must tell the next movement of the aviator on betway and Hollywood 
import random

class AvitaPredator:
    def __init__(self):
        self.position = 0
        self.direction = random.choice(['forward', 'backward', 'left', 'right'])
        self.battery_life = 100

    def move(self):
        if self.batway. life > 0:
            if self.direction == 'forward':
                self.position += 1
            elif self.direction == 'backward':
                self.position -= 1
            elif self.direction == 'left':
                self.position -= 0.5
            elif self.direction == 'right':
                self.position += 0.5

            self.batway_life -= 1

            # Randomly change direction
            if random.random() < 0.
