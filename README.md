# kilo2-Day2

What did I learn?

1.get user input from textfield!
->>> this is textfield properties
``` 
TextField(
                controller: controller,
                textAlign: TextAlign.center,
                decoration: const InputDecoration(hintText: '\$100.00'),
                keyboardType:
                    const TextInputType.numberWithOptions(decimal: true),
              )
```

before we need to create 
final controller = TextEditingController();
in textfield we have property called controller we neeed to assign our controller to it. 


2.  
```
if (tip != null)
              Text(
                tip!,
                style:
                    const TextStyle(fontSize: 30, fontWeight: FontWeight.bold),
              ),
```
it means -> show only there is a value(it is not null) otherwise show nothing

3. ToggleButton
```
 ToggleButtons(
              fillColor: Colors.black,
              selectedColor: Colors.white,
              children: const [
                Text('10%'),
                Text('20%'),
                Text('30%'),
              ],
              isSelected: isSelected,
              onPressed: updateSelection,
            ),
            ```

<img width="1440" alt="image" src="https://user-images.githubusercontent.com/60324587/178655839-8d8f3b83-15fa-4d37-b955-0ae198e275a7.png">


