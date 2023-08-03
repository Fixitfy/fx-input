# fx-input
RedM Input System

# insatallation

- `ensure fx-input` in the top of your resources.cfg 

# features
- Custom designe Fixitfy
- Very easy to use

# Credit
* credit goes to the QBCORE and RSGCore team for basecode and functionality
# Example
```lua
RegisterCommand('testinput', function(args)
    local dialog = exports['fx-input']:ShowInput({
        header = 'Target Player ID: 3',
        submitText = "Confirm",
        inputs = {
            {
                type = 'number',
                name = 'playercash',
                text = 'Player Cash: 2500 $',
                isRequired = false,
            },
            {
                type = 'number',
                name = 'playergold',
                text = 'Player Gold: 0',
                isRequired = false,
            }
        }
    })
    if dialog then
        print(json.encode(dialog))
    end
end)
```
# Media
![Screenshot_371](https://github.com/Fixitfy/fx-input/assets/139653962/1ef27c12-b23f-43e9-a198-0ad438dcafbb)
