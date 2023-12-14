
<div align="center">
  <h1 align="center">StackOverBot</h1>

  <p align="center">
    A discord bot to search Stack Overflow questions written in Python.
  </p>
</div>

## Preview
![](https://i.ibb.co/VWXPGW5/image-2022-05-07-202341359.png)
![](https://i.ibb.co/PG68bZm/image-2022-05-07-002807207.png)

*Click the ⏭ to show the next question !*


### Built With / Interact with
* ![Py](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)
* ![Docker](https://img.shields.io/badge/RStudio-75AADB?style=for-the-badge&logo=RStudio&logoColor=white)
* ![stack](https://img.shields.io/badge/Stack_Overflow-FE7A16?style=for-the-badge&logo=stack-overflow&logoColor=white)
* ![discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)


## Usage

**Bot token can be stored in separated `.env` file in a `env` folder at the root of the repository**

Perform comunication with the discord API with : [Pycord](https://github.com/Pycord-Development/pycord)


## Build Docker

Build image using : 
```
$    docker build -t stackoverbot .
```
Run container using : 
```
$   docker run \
    -d --restart unless-stopped \
    -e DISCORD_TOKEN="your_token" \
    -e DISCORD_DEBUG_GUILD="guild_debug_id" \
    --name container_name \
    stackoverbot
```
⚠ `DISCORD_DEBUG_GUILD` is not mandatory (This is to update the bot only in the specified server, avoiding to wait for change propagation)

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "improvement".
Don't forget to give the project a star! Thanks again!

## License

License : [DBAD](https://github.com/philsturgeon/dbad)
Distributed under the GNU General Public License v3.0. See `LICENSE` for more information.












