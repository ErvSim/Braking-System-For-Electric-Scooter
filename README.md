Fuzzy logic implementation is a method in control systems that mimics human reasoning by handling uncertainty and imprecision. Instead of binary true/false values, it assigns degrees of truth to variables, enabling smooth, adaptive responses to real-world inputs. It is commonly used in systems like automatic braking or temperature control, where precise, flexible decision-making is required in varying conditions. The project done here is a braking system for an entry level electric scooter in perfect condition.

Using MATLAB's fuzzyLogicDesigner, we developed a Mamdani Type-1 FIS (Fuzzy Inference System) with three input variables and one output. A key advantage of fuzzy logic is its flexibility, allowing us to design our system based on expert knowledge and intuition rather than requiring precise data. This approach enables our project to function effectively even with incomplete information. 

Our first input is speed. Based on our research, entry-level scooters typically operate between 15 and 25 mph, but we set a maximum of 30 mph as a precaution. Using our intuition, we defined membership functions to classify speeds as slow, medium, or fast. The fuzzyLogicDesigner software then adjusts these functions according to our rule set. We applied this approach consistently across all inputs and the output.

<img src="https://github.com/user-attachments/assets/a2c4ab98-e10c-44f8-a10c-f6463e8f7fd0" height="100%" width="100%" alt="Disk Sanitization Steps"/>
---

<br />Our next input is distance, ranging from 0 to 50 feet. This range is primarily based on our experience rather than formal research.


<img src="https://github.com/user-attachments/assets/a5d37a69-66ea-41a7-8c18-88f85f3325db" height="100%" width="100%" alt="Disk Sanitization Steps"/>


Our final input is weight. Instead of typical light, medium, and heavy categories, we focused on the maximum weight limit of 220 lbs, which is common for entry-level scooters. Exceeding this limit significantly increases braking distance, often doubling or more. It’s important to note that weight limits vary across scooter types, so our input applies specifically to scooters rated for 220 lbs or less.
<br />

<img src="https://github.com/user-attachments/assets/f5090244-f8a3-44e7-8434-7c1e6a5fd24a" height="100%" width="100%" alt="Disk Sanitization Steps"/>


Our output is the recommended braking force, expressed as a percentage. This choice was based on our intuition rather than formal research, allowing our design to be adaptable to any scooter. Although some brake types perform better than others, we included a 5% margin of error to account for these differences, making our approach versatile. This flexibility proved especially useful given the lack of specific research on braking force values and units for scooters.
<br />

<img src="https://github.com/user-attachments/assets/7582b34b-4c2d-49ba-a044-96db5d487cac" height="100%" width="100%" alt="Disk Sanitization Steps"/>

Using specific membership functions for each input, we created a set of rules that determine the output—in this case, the braking force percentage—based on selected inputs. While we aimed for a sufficient number of rules, we avoided excess, as more rules do not necessarily improve a fuzzy logic system. These rules were crafted intuitively rather than data-driven. Once established, MATLAB interprets these rules to generate a 3D graph, helping us visualize relationships between inputs and outputs. We then debugged the rules to ensure the 3D graph is smooth, with no unexpected dips or bumps that would indicate conflicting rules.
<br />

<img src="https://github.com/user-attachments/assets/31ad4cb1-a2f8-4d0d-9e98-060ea05da270" height="100%" width="100%" alt="Disk Sanitization Steps"/>

With the necessary data inputted into fuzzyLogicDesigner, MATLAB applies clipping and defuzzification methods to generate our output. It combines all inputs and outputs to produce a 3D representation of the system, visualizing how each variable influences the braking force percentage. Shown below are the 3D visuals for Speed vs. Distance, Speed vs. Weight, and Distance vs. Weight, respectively. This graph effectively demonstrates the overall behavior and interaction of inputs in our fuzzy logic model.
<br />

<img src="https://github.com/user-attachments/assets/f3725c03-2769-46f4-a835-5755d4a73471" height="100%" width="100%" alt="Disk Sanitization Steps"/>

<br />

<img src="https://github.com/user-attachments/assets/eaa8493f-d842-4c89-ab41-3da67b95e0b1" height="100%" width="100%" alt="Disk Sanitization Steps"/>

<br />

<img src="https://github.com/user-attachments/assets/b60fa672-fedc-41b9-b5fe-ca3e9e3049c5" height="100%" width="100%" alt="Disk Sanitization Steps"/>

Due to defuzzification, our system cannot reach the absolute maximum or minimum values; achieving these extremes would require normalization or extending the input ranges. Alongside the 3D visualization, we also used the "rule inference" tool, which allows us to select specific input values and observe the resulting output. This tool is especially useful for debugging, as it highlights which rules influence the output, helping us identify any conflicting rules. Additionally, if we need a specific output value, we can simply enter desired input values to obtain the exact output without searching through the 3D graph.
<br />

<img src="https://github.com/user-attachments/assets/2b474ead-d936-44af-9b1d-f5824990aed3" height="100%" width="100%" alt="Disk Sanitization Steps"/>
