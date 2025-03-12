# Function Playground

![function logo](https://raw.githubusercontent.com/fxnai/.github/main/logo_wide.png)

[![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fdiscord.com%2Fapi%2Finvites%2Fy5vwgXkz2f%3Fwith_counts%3Dtrue&query=%24.approximate_member_count&logo=discord&logoColor=white&label=Function%20community)](https://fxn.ai/community)

This project demonstrates the process of compiling a Python function then running it in the following frameworks: 
- React (Browser, Node.js)
- React Native (Android, iOS)
- Kotlin in Android Studio (Android)
- Swift in Xcode (iOS)
- Python (Linux, macOS, Windows)
- Unity Engine (Android, iOS, Linux, macOS, visionOS, WebGL, Windows)

## Setup Instructions
First, download the Function CLI:
```bash
# 💥 Install the Function CLI
$ pip install --upgrade fxn
```

Next, create an [access key](https://fxn.ai/settings/developer) and login to the CLI:
```bash
# 🔥 Login to the Function CLI
$ fxn auth login <ACCESS KEY>
```

## Compiling your Function
The [predictor.py](predictor.py) module defines a prediction function `greeting`. Update the predictor `tag` 
with your Function username:
```py
from fxn import compile

@compile(
    tag="@your-username/greeting", # replace `your-username`
    description="Say a friendly greeting."
)
def greeting (name: str) -> str:
    return f"Hey there {name}! We're glad you're using Function and we hope you like it."
```

Compile it using the `fxn compile` CLI command:
```bash
# Compile the `greeting` function
$ fxn compile predictor.py
```

## Using the Function
See the respective directories for more information.

## Useful Links
- [Discover predictors to use in your apps](https://fxn.ai/explore).
- [Join our Discord community](https://discord.gg/fxn).
- [Check out our docs](https://docs.fxn.ai).
- Learn more about us [on our blog](https://blog.fxn.ai).
- Reach out to us at [stdin@fxn.ai](mailto:stdin@fxn.ai).

Function is a product of [NatML Inc](https://github.com/natmlx).