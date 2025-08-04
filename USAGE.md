<!-- Start SDK Example Usage [usage] -->
```python
# Synchronous Example
from nest_api import NestAPI


with NestAPI() as na_client:

    res = na_client.git_hub.list_issues(page=1)

    # Handle response
    print(res)
```

</br>

The same SDK client can also be used to make asychronous requests by importing asyncio.
```python
# Asynchronous Example
import asyncio
from nest_api import NestAPI

async def main():

    async with NestAPI() as na_client:

        res = await na_client.git_hub.list_issues_async(page=1)

        # Handle response
        print(res)

asyncio.run(main())
```
<!-- End SDK Example Usage [usage] -->