# unemployment-inclass-summer-2023



## Setup

Obtain an [AlphaVantage API Key](https://www.alphavantage.co/support/#api-key). A normal key should be fine, but alternatively you can use one of the prof's "premium" keys. Then create a file called ".env" and place it inside (the following example):

```ALPHAVANTAGE_API_KEY="_____"

```

Create a virtual environment:

```sh
conda create -n unemployment-env python=3.10
```

```sh
conda activate unemployment-env
```

Install third-party packages:

```sh
pip install -r requirements.txt
```

## Usage

Run the report:

```sh
python app/unemployment.py

python -m app.unemployment
```

Run the web app:
# ... if `export` doesn't work for you, try `set` instead
# ... or try a ".env" file approach
export FLASK_APP=web_app flask run

Run the stocks report:

```sh
python -m app.stocks
```

## Testing

Run tests:

```sh
pytest
```


## [Deployment Guide](/DEPLOYING.md)