# AWS Bedrock Router Evaluation

This repository contains sample notebooks to demonstrate how to evaluate an LLM-augmented system. It provides tools and methods for local evaluation.

## Environment
1. Ensure you've enabled Amazon Titan Embedding models as well as Claude Sonnet and Claude Haiku in the Bedrock Console.
2. Ensure you have adequate permissions to call Bedrock from the Python SDK (Boto3)

### Local
These notebooks were tested with Python 3.10 and higher. If you're running locally, ensure you're using >3.10. Also ensure that you have the AWS CLI setup with the credentials you want set to the default profile. These credentials need access to Amazon Bedrock Models.

### Details

- `data/`: Contains the datasets 
- `notebooks/`: Jupyter notebooks demonstrating the routers and evaluation


## Getting Started

1. Clone the repository:
   ```
   git clone https://github.com/fhuthmacher/aws-bedrock-router-eval.git
   cd aws-bedrock-router-eval
   ```

2. Set up a virtual environment:
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

   or create a conda environment

   ```
   conda create -y --name bedrock-router-eval python=3.11.8
   conda init && activate bedrock-router-eval
   conda install -n bedrock-router-eval ipykernel --update-deps --force-reinstall -y
   conda install -c conda-forge ipython-sql
   ```

3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

4. Start at notebook 1 and work your way through them!

## Usage

1. Explore the example notebooks in the `example-notebooks/` directory to understand different evaluation techniques.

## Authors

- Clement Perrot - *Initial work* - [github](https://github.com/clemfeelsgood)
- Felix Huthmacher  - *Initial work* - [github](https://github.com/fhuthmacher)

## License

This library is licensed under the MIT-0 License. See the LICENSE file.