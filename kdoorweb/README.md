# K-Door-web

# Development setup

    python3 -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt

## Initialize database

    source venv/bin/activate



## Run dev server

    source venv/bin/activate
    bottle.py --debug --reload kdoorweb:application

## Run unittests

    source venv/bin/activate
    python -m unittest discover tests

## Update requirements.txt

    source venv/bin/activate
    pip-compile --upgrade setup.py
    pip-compile --upgrade dev-requirements.in
    # Apply updates to current venv
    pip-sync dev-requirements.txt requirements.txt