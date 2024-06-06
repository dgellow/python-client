# Mixpeek SDK

A Python SDK for the Mixpeek API.

## Installation

```bash
pip install mixpeek
```

```python
from mixpeek import Mixpeek
from pydantic import BaseModel

mixpeek = Mixpeek("YOUR_API_KEY")

# Example usage
extraction = mixpeek.extract.text(
    input="s3://document.pdf",
    input_type="url"
)

embedding = mixpeek.embed.video(
    model="mixpeek/vuse-generic-v1",
    input="s3://waving_boy.mp4",
    input_type="url"
)

class ResponseFormat(BaseModel):
    city: int
    weather: float

generated_content = mixpeek.generate.text(
    response_format=ResponseFormat,
    context="Please tell me the weather and make sure to respond in the provided JSON schema"
)

mixpeek.create_connection(
    alias="my-mongo-test",
    engine="mongodb",
    details={
        "host": "your_host_address",
        "database": "your_database_name",
        "username": "your_username",
        "password": "your_password"
    }
)

response = mixpeek.tools.video.process(
    url="https://s3/video.mp4",
    frame_interval=5,
    resolution=[720, 1280],
    return_base64=True
)
```
