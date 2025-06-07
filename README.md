# PraisonAI 🤖✨

![PraisonAI](https://img.shields.io/badge/PraisonAI-Ready-blue.svg)  
[![Latest Release](https://img.shields.io/github/v/release/mbabazii/PraisonAI)](https://github.com/mbabazii/PraisonAI/releases)

Welcome to **PraisonAI**, a powerful framework designed for creating and managing multiple AI agents. This repository aims to simplify the development of AI systems, enabling you to automate tasks and solve complex challenges with ease.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

PraisonAI is a production-ready multi-agent framework that focuses on providing a low-code solution. Whether you want to build simple automation tools or tackle intricate problems, this framework helps streamline the process. It emphasizes simplicity, customization, and effective collaboration between humans and agents.

For the latest updates, check the [Releases](https://github.com/mbabazii/PraisonAI/releases) section.

## Features

- **Multi-Agent Support**: Easily create and manage multiple AI agents.
- **Low-Code Development**: Build applications with minimal coding effort.
- **Customizable**: Tailor agents to fit your specific needs.
- **Human-Agent Collaboration**: Enhance productivity through effective teamwork.
- **Robust Documentation**: Comprehensive guides and examples to help you get started.

## Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- Python 3.7 or later
- pip (Python package installer)

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/mbabazii/PraisonAI.git
   ```

2. Navigate to the project directory:

   ```bash
   cd PraisonAI
   ```

3. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

### Quick Start

To get started quickly, you can run the example provided in the `examples` folder. Navigate to the folder and execute the following command:

```bash
python example.py
```

This will demonstrate how to set up a basic multi-agent system.

## Usage

PraisonAI allows you to create agents for various tasks. Here’s a simple example to illustrate how to define an agent.

### Creating an Agent

You can define an agent by creating a new class that inherits from the base agent class. Here’s a basic example:

```python
from praisonai import Agent

class MyAgent(Agent):
    def perform_task(self, task):
        # Your task logic here
        return f"Task {task} completed!"
```

### Running Agents

Once you define your agents, you can run them in a multi-agent system:

```python
from praisonai import MultiAgentSystem

system = MultiAgentSystem()
agent1 = MyAgent(name="Agent1")
agent2 = MyAgent(name="Agent2")

system.add_agent(agent1)
system.add_agent(agent2)

system.run()
```

### Collaboration Between Agents

PraisonAI allows agents to communicate with each other. Here’s how you can implement collaboration:

```python
class CollaborativeAgent(Agent):
    def communicate(self, message):
        # Logic for communication
        return f"Received message: {message}"

agent1 = CollaborativeAgent(name="Agent1")
agent2 = CollaborativeAgent(name="Agent2")

response = agent1.communicate("Hello from Agent1!")
print(response)
```

## Contributing

We welcome contributions to enhance the functionality of PraisonAI. Here’s how you can contribute:

1. **Fork the Repository**: Click on the "Fork" button at the top right corner of the page.
2. **Create a Branch**: Create a new branch for your feature or bug fix.
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Make Changes**: Implement your changes and test them thoroughly.
4. **Submit a Pull Request**: Push your changes and submit a pull request for review.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries or support, feel free to reach out:

- **Email**: your-email@example.com
- **GitHub**: [mbabazii](https://github.com/mbabazii)

For the latest updates, check the [Releases](https://github.com/mbabazii/PraisonAI/releases) section.

---

PraisonAI aims to make AI agent development accessible and efficient. We hope you find this framework useful for your projects. Happy coding!