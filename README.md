# Asynchronous-
Asynchronous Programming using asyncio:
import asyncio

async def async_function():
    print("Start async function")
    await asyncio.sleep(2)
    print("Async function completed")

async def main():
    print("Start main function")
    await asyncio.gather(async_function(), async_function())
    print("Main function completed")

asyncio.run(main())
