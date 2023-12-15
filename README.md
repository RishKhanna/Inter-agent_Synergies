# Inter-agent Synergies

## Learning Inter-Agent Synergies in Asymmetric Multiagent Systems

This project implements the Asymmetrical Island Model (AIM) for solving the Habitat Problem, as presented in the paper titled "Learning Inter-Agent Synergies in Asymmetric Multiagent Systems" by Gaurav Dixit and Kagan Turner at AAMAS 2023.

### Implementation

The AIM model for the Habitat Problem is implemented in Python. The project includes classes for each agent type, namely Rovers, Excavators, and Drones.

#### Agent Classes

- **Rover:** Represents the rover agent, and has the sensing equipment.
- **Excavator:** Represents the excavator agent, and has the digging equipment.
- **Drone:** Represents the drone agent, and has the communication infrastructure.

#### Team Class

A team is a collection of agents from the various classes. Teams are stored in lists, with separate lists for rovers, excavators, and drones.

#### Mainland Class

The Mainland class defines the characteristics of the mainland, including team size, population size (number of teams in the mainland), the number of elite teams, and habitat-specific data such as habitat extents and the number of dig sites.

### Policy Migration

The policy migration process integrates the operation of Islands and Mainlands in the Asymmetrical Island Model. It consists of the following four main steps:

1. **SoftMax Function Definition:** Defines the SoftMax function.
2. **Island Optimization:** Optimizes the policies of each island for a specified number of iterations using functions defined within the island class.
3. **Elite Team Selection:** Selects elite teams from each mainland, and appends the agent policies of these teams to the current population of islands.
4. **Weight Update:** Updates the weights associated with the SoftMax function based on a gradient derived from the agents' performances on the mainland in the current iteration.

### Contributions from the Base Paper

The project incorporates the three-step algorithm proposed in the base paper:

1. **Quality Diversity on Islands:** Implemented the algorithm to perform quality diversity on islands.
2. **Evolutionary Optimization on Mainlands:** Implemented evolutionary optimization on mainlands.
3. **Policy Migration:** Implemented policy migration between islands and mainlands.

Additionally, various game modes (Decay, Volatile, Mixed) have been implemented to test the agents in challenging environments. The project evaluates the model based on three metrics proposed in the paper:

1. **Asymmetric Coordination**
2. **Adaptability to Unseen Tasks**

Rollouts based on the algorithm have been performed to assess the effectiveness of the model in achieving the objectives outlined in the paper.

Feel free to explore the codebase and adapt it to your specific needs. For any questions or issues, please refer to the documentation or contact the project maintainers.

# Contribution
- [Aadarsh Ragunathan]()
- [Bhumika Joshi]()
- [Rishabh Khanna](https://github.com/RishKhanna/)
