# develojoping
In the context of the profile as a whole, the "develojoping-ment" can be seen as a rough draft, for now, even if it may not follow the best approach completely. But this is not a big issue as long as the end result is not greatly affected. This initial section is dedicated to comprehending not only the programs and the code itself, but also, in principle, the underlying platforms and mechanisms of operation. After all, this is the first project, I was just learning and figuring things out. to repeat at my own risk, although mine are few if not none - after this short introduction, I attach all the materials that I have relied on and used. To be honest, there is more info than even needs for beginning, just be patient and attentive, and especially to these particularly helpful sources (libs and step-by-step tutorials). 

[github.com/openai/openai-quickstart-python](https://github.com/openai/openai-quickstart-python)

# OpenAI API Quickstart - Python

This repository hosts multiple quickstart apps for different OpenAI API endpoints (chat, assistants, etc). Check out the `examples` folder to try out different examples and get started using the OpenAI API.

## Basic request

To send your first API request with the [OpenAI Python SDK](https://github.com/openai/openai-python), make sure you have the right [dependencies installed](https://platform.openai.com/docs/quickstart?context=python) and then run the following code:

```python
from openai import OpenAI
client = OpenAI()

completion = client.chat.completions.create(
  model="gpt-3.5-turbo",
  messages=[
    {"role": "system", "content": "You are a helpful assistant."},
    {"role": "user", "content": "Hello!"}
  ]
)

print(completion.choices[0].message)
```

## Setup

1. If you don’t have Python installed, install it [from Python.org](https://www.python.org/downloads/).

2. [Clone](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) this repository.

3. Navigate into the project directory:

   ```bash
   $ cd openai-quickstart-python
   ```

4. Create a new virtual environment:

   - macOS:

     ```bash
     $ python -m venv venv
     $ . venv/bin/activate
     ```

   - Windows:
     ```cmd
     > python -m venv venv
     > .\venv\Scripts\activate
     ```

5. Install the requirements:

   ```bash
   $ pip install -r requirements.txt
   ```

6. Make a copy of the example environment variables file:

   ```bash
   $ cp .env.example .env
   ```

7. Add your [API key](https://platform.openai.com/api-keys) to the newly created `.env` file.

8. Run the app:

This step depends on the app itself. If the code uses flask (like the chat-basic example), you can run:

```bash
$ flask run
```

You should now be able to access the app from your browser at the following URL: [http://localhost:5000](http://localhost:5000)!



If the code is just a simple Python script, you can run it with:

```bash
$ python my_file.py
```
LICENSE here is similiar with what i got, because i have no idea which one i need.
