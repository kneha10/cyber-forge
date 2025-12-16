🛡️ CyberForge - Breach Probability Simulator

CyberForge is an interactive risk quantification dashboard for cybersecurity professionals. It helps CISOs and Security Architects visualize the concept of Defense in Depth and communicate the ROI of security investments.

It simulates how specific controls (like MFA or Zero Trust) reduce the mathematical probability of a breach against varying levels of threat sophistication.
✨ Key Features

    Threat Actor Simulation: Adjust the adversary from "Script Kiddie" to "APT Group" to see how risk profiles change based on attacker capability.

    Defense Stack Builder: Toggle active countermeasures (MFA, EDR, Patching) to observe the immediate impact on the risk curve.

    Poisson Breach Modeling: Uses standard risk quantification math (P=1−e−λt) to model the "Time to Compromise."

    SOC Aesthetic: Designed with a dark-mode, terminal-inspired UI to match standard InfoSec tooling.

🚀 Quick Start

    Load: Open index.html in any browser.

    Define Threat: Use the "Attacker Sophistication" slider to set the scenario (e.g., Ransomware Gang).

    Build Defenses: Click on the tiles in the "Defense Stack" to activate them.

        Try enabling MFA + EDR to see the curve flatten.

    Assess: Review the "Breach Probability (24h)" and "Est. Impact Cost" KPIs.

🧮 The Logic: Risk Quantification

The simulator treats a cyberattack as a stochastic process.
Risk=(Threat×Vulnerability)×(1−Mitigation)

    Threat: Defined by the sophistication slider.

    Mitigation: Defined by the Defense Stack. Each layer applies a reduction multiplier (e.g., MFA reduces remaining risk by 45%).

    Curve: The chart plots the cumulative probability of a successful compromise over a 24-hour window of sustained attack.

⚙️ Configuration

The efficacy of security controls is defined in the DEFENSES constant. You can adjust these values based on your organization's specific toolset efficacy.
JavaScript
