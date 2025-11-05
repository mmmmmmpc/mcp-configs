# mcphost-configurations

A community-driven collection of configuration files for the `mcphost` utility in SUSE Linux Enterprise Server 16 (SLES 16). This project aims to provide ready-to-use configs for connecting SLESi 16 to various Large Language Models (LLMs).

---

## 🚀 What is mcphost?

SLES 16 introduces `mcphost`, a powerful command-line utility designed to bridge the gap between your enterprise server and the world of Generative AI. It allows you to query Large Language Models (LLMs) directly from the SLES environment, enabling automation, scripting, assisted troubleshooting and integration of AI capabilities into your system workflows.

## 🎯 Purpose of This Repository

While `mcphost` provides the connection, each LLM provider requires specific configuration details, such as API endpoints, authentication methods, and model parameters. This repository serves as a central, community-maintained collection of pre-built configuration files to help you get connected quickly.

---

## 📂 Included Configurations

This repository is just starting! The initial configuration provided is:

* **Google Gemini 2.5 Pro**
    * **File:** `gemini-2.5-pro_mcp.yaml`
    * **Auth Method:** Auth Token (API Key)
    * **Description:** A baseline configuration to connect to Google's Gemini 2.5 Pro model using a standard API key.

---

## 🔧 How to Use

### 1. Prerequisites

* A running instance of **SLES 16** already registered to SCC and up to date.
* Install `mcphost` utility by running `zypper in mcphost`
* Get an active **API Key (Auth Token)** from the respective LLM provider (e.g., Google AI Studio for Gemini).

### 2. Configuration

1.  **Clone this repository:**
    ```bash
    git clone [https://github.com/mmmmmmpc/mcp-configs.git](https://github.com/mmmmmmpc/mcp-configs.git)
    cd mcp-configs
    ```

2.  **Copy the desired configuration:**
    The default `mcphost` configuration is typically located at `~/.mcp.yaml` or `~/mcp.json`. You can copy the configuration from this repo to that location.

    ```bash
    # Example for the Gemini 2.5 Pro config
    cp gemini-2.5-pro_mcp.yaml ~/.mcp.yaml

3.  **Run mcphost**
    Run `mcphost` in the command line an check all options are properly loading.

