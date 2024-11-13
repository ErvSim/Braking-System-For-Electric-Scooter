<br />

<img src="" height="20%" width="50%" alt="Disk Sanitization Steps"/>

<br />

<img src="" height="20%" width="50%" alt="Disk Sanitization Steps"/>

<br />

<img src="" height="20%" width="50%" alt="Disk Sanitization Steps"/>
<br />

<img src="" height="20%" width="50%" alt="Disk Sanitization Steps"/>
<br />

<img src="" height="20%" width="50%" alt="Disk Sanitization Steps"/>
<br />

<img src="" height="20%" width="50%" alt="Disk Sanitization Steps"/>

<br />

<img src="" height="20%" width="50%" alt="Disk Sanitization Steps"/>

<br />

<img src="" height="20%" width="50%" alt="Disk Sanitization Steps"/>

<br />

<img src="" height="20%" width="50%" alt="Disk Sanitization Steps"/>

<br />

<img src="" height="20%" width="50%" alt="Disk Sanitization Steps"/>








Fuzzy logic implementation is a method in control systems that mimics human reasoning by handling uncertainty and imprecision. Instead of binary true/false values, it assigns degrees of truth to variables, enabling smooth, adaptive responses to real-world inputs. It is commonly used in systems like automatic braking or temperature control, where precise, flexible decision-making is required in varying conditions. The project done here is a braking system for an entry level electric scooter in perfect condition.

Using MATLAB's fuzzyLogicDesigner, we developed a Mamdani Type-1 FIS (Fuzzy Inference System) with three input variables and one output. A key advantage of fuzzy logic is its flexibility, allowing us to design our system based on expert knowledge and intuition rather than requiring precise data. This approach enables our project to function effectively even with incomplete information. 

Our first input is speed. Based on our research, entry-level scooters typically operate between 15 and 25 mph, but we set a maximum of 30 mph as a precaution. Using our intuition, we defined membership functions to classify speeds as slow, medium, or fast. The fuzzyLogicDesigner software then adjusts these functions according to our rule set. We applied this approach consistently across all inputs and the output.
<br />

<img src="https://github.com/user-attachments/assets/a2c4ab98-e10c-44f8-a10c-f6463e8f7fd0" height="100%" width="100%" alt="Disk Sanitization Steps"/>


Our next input is distance, ranging from 0 to 50 feet. This range is primarily based on our experience rather than formal research.
<br />

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
