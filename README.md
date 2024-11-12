<br />

<img src="" height="20%" width="50%" alt="Disk Sanitization Steps"/>

<br />

<img src="" height="20%" width="50%" alt="Disk Sanitization Steps"/>

<br />

<img src="" height="20%" width="50%" alt="Disk Sanitization Steps"/>






Fuzzy logic implementation is a method in control systems that mimics human reasoning by handling uncertainty and imprecision. Instead of binary true/false values, it assigns degrees of truth to variables, enabling smooth, adaptive responses to real-world inputs. It is commonly used in systems like automatic braking or temperature control, where precise, flexible decision-making is required in varying conditions. The project done here is a braking system for an entry level electric scooter.

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
