# Terminal Orchestrator

Terminal Orchestrator is a Windows desktop workspace for planning tasks with an AI model and delegating them to coding agents. Choose a local or cloud model, give an executor a role, and inspect its output and file checks in the conversation.

## Download and run

1. Download [the clean source archive](../../raw/refs/heads/main/terminal-orchestrator-github.zip) and extract it. Open PowerShell in the extracted folder containing `desktop.py`.
2. With Python 3.11 or newer installed, run the commands below. The interface opens in Edge or Chrome.

```powershell
python -m venv .venv
.venv\Scripts\python.exe -m pip install -r requirements.txt
.\START.cmd
```

3. Open **Настройки → Подключения ИИ** and add your first model. Supply your provider URL, model ID and credentials. For a local model, configure your own Ollama server.
4. In **Агенты**, check which CLI programs the application detects. Install and authorize your preferred agent separately, then choose its role under **Исполнители**. You can also register a custom CLI.

The source archive includes the Windows application, web interface, configuration examples, documentation and tests. The default model list is empty. Access to project files is controlled from the chat. Automatic mode delegates subtasks sequentially. Supported adapters include OpenCode, Hermes Agent, DeepSeek Harness, Aider, Codex CLI, Claude Code and Kimi Code.

## По-русски

[Скачайте архив с исходниками](../../raw/refs/heads/main/terminal-orchestrator-github.zip), распакуйте и выполните команды выше. В архиве есть подробный README на русском, инструкции по настройке агентов и сборке EXE. При первом запуске добавьте свою модель и выберите права доступа внизу чата. Для проверки результата смотрите журнал исполнителя и созданные файлы.

The archive contains adapters for external tools. Each tool and model service has its own installation, authorization and license terms. The project owner has not selected a distribution license for the orchestrator yet.
