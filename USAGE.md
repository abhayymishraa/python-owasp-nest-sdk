<!-- Start SDK Example Usage [usage] -->
```python
# Synchronous Example
from nest_sdk_python_test_v1 import NestAPI


with NestAPI() as nest_api:

    res = nest_api.git_hub.list_issues(page=1)

    # Handle response
    print(res)
```

</br>

The same SDK client can also be used to make asychronous requests by importing asyncio.
```python
# Asynchronous Example
import asyncio
from nest_sdk_python_test_v1 import NestAPI

async def main():

    async with NestAPI() as nest_api:

        res = await nest_api.git_hub.list_issues_async(page=1)

        # Handle response
        print(res)

asyncio.run(main())
```
<!-- End SDK Example Usage [usage] -->