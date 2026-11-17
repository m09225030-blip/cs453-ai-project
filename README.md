CS453 - Individual AI Project: After-Hours Cleaning Robot

Name: إنتصار محمد معيتيق
Student ID: 09225030
Project: After-Hours Cleaning Robot
Variant: 1
Closed road: B – E
Target room: F
Route to clean: S → A → C → F (3 moves)

What this project does

A cleaning robot starts at location S on a small campus map containing 8 locations. One road is closed according to the student's assigned variant. The robot must reach its assigned target room F and clean it.

The project models the task using PEAS, state representation, actions, transitions, and costs. It then simulates the robot's mission using two search algorithms:

- BFS (Breadth-First Search): An uninformed search algorithm that finds a route with the fewest moves.
- A Search:* An informed search algorithm that uses a heuristic to guide the search toward the goal.

Both algorithms find a route with the same minimum number of moves on the assigned map.

The simulator executes the route, performs the cleaning action, and verifies that the task is complete.

Files

- "project.ipynb" – The complete notebook containing the project implementation and explanations.
- "README.md" – Project description and instructions.

Dependencies

Python 3 and its standard library only:

- copy
- collections
- heapq
- platform

No additional installations, GPU, API keys, or physical robot are required.

How to run

1. Open "project.ipynb" in Google Colab.
2. Check that "STUDENT_ID" is set to ""09225030"", preserving the leading zero.
3. Select Runtime → Restart session and run all.
4. Check the BFS and A* outputs.
5. Verify that the robot reaches room F, performs the cleaning action, and displays "Task complete: True".

Sources and AI assistance

The reference graph, variant helper, and heuristic tables are provided by the CS453 two-week project workbook.

AI assistance was used to help draft explanations and develop parts of the implementation. The code was reviewed and tested using the provided edge cases, including start equals goal, unreachable goals, invalid locations, and illegal or repeated cleaning actions.

The BFS and A* implementations were checked by comparing their minimum route costs and verifying the heuristic's admissibility and consistency on the assigned map.

Colab link

https://colab.research.google.com/github/m09225030-blip/-/blob/master/project.ipynb
