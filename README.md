# 🌟 Crumbs: Dynamic Trivia via Notifications 🌟

## 📜 Description

Crumbs utilizes LLMs to deliver periodic customizable trivia
facts to you. Whether you're a trivia enthusiast or just looking for a fun and
lightweight way to learn new things, Crumbs has got your back!

## 🚀 Features

- **Trivia Fact Generation:** Utilizes OpenAI's API to generate trivia facts. You could use your own large language model as well, whether locally or from HuggingFace.
- **Smart Deduplication:** Employs TF-IDF and cosine similarity to avoid repetitive facts.
- **System Notifications:** Delivers facts directly to your Macbook's notifications.
- **Dynamic Scheduling:** Operates within specified hours, suitable for daily routines.
- **Non-invasive:** Crumbs runs super quietly in the background and uses virtually no resources. You can monitor this by searching "python" in Activity Monitor. Look for the job number corresponding to this script via

```zshrc
$ jobs -l
[1]  + [No. here] running    nohup python breadcrumbs.py
```

## 🔧 Installation

### Prerequisites

- Python 3.x 🐍
- Pip (Python package installer)

### Setup

1. Clone the repository:

   ```zshrc
   $ git clone https://github.com/windsornguyen/crumbs.git
   ```

2. Navigate to the cloned directory:

   ```zshrc
   $ cd crumbs
   ```

3. Install the required packages:

   ```zshrc
   $ pip install -r requirements.txt
   ```

### Usage

1. Set your OpenAI API key in an .env file:

   ```zshrc
   API_KEY=your_openai_api_key_here
   ```

2. Run the script in the background:

    ```zshrc
    nohup python crumbs.py &
    ```

### Contributing

Contributions to Crumbs are welcomed, and in fact, encouraged! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch

```zshrc
git checkout -b feature-branch
```

3. Make your changes and commit them

```zshrc
git commit -am "Added some features!"
```

4. Push to the branch

```zshrc
git push origin feature-branch
```

5. Create a new Pull Request.

### License

This project is licensed under the MIT License. See the LICENSE.md file for details.

### Acknowledgements

- OpenAI for providing their amazing API. We love the OpenAI team so much. OpenAI is nothing without its people. ❤️
- Contributors and maintainers of the Python packages used in this project.

### Note

This project is not affiliated with OpenAI and uses its API under their terms and conditions.
