+++
author = "Abdurrahman Rajab"
title = "Whisper on windows command line"
date = "2023-01-1"
description = "A short guide on how to use whisper on windows!"
tags = [
    "Open Source",
    "openAI",
    "whisper",
]
categories = [
    "Open source",
    "openAi",
    "GitHub"
]
+++

Whisper is OpenAI speech to text model, this short blog will show you how to run it on windows assuming you are using it for the first time.

Before you use whisper you need to make sure to have: 

- Python: you can get it from [MSFT Store](https://apps.microsoft.com/store/detail/python-39/9P7QFQMJRFP7?hl=en-us&gl=us). 
- Git: from the [official website](https://git-scm.com/downloads). 
- [Choco](https://chocolatey.org/) or [scoop](https://scoop.sh/): you can check the default websites for further details.

After making sure you have those you can follow the details on the [official whisper repo](https://github.com/openai/whisper) at GitHub then,do the next:

To run it from the CMD you need to have a virtual environment for python which you can learn more about it from this [the official python docs](https://docs.python.org/3/library/venv.html), but in short it will be the next: 

```cmd
python3 -m venv /path/to/new/virtual/environment
```

from powershell: 

```cmd
PS C:\> <venv>\Scripts\Activate.ps1
```

make sure to write the path you want to have the environment in it in the first command, and you need to use it in the second one.