FROM fastapi:dev

RUN apt-get update && apt-get -y upgrade
RUN pip install --upgrade pip poetry

ENTRYPOINT ["poetry", "run", "uvicorn", "api.main:app", "--host", "0.0.0.0", "--reload"]