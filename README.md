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
so, basically toggle button gives us easy option to choose, (not difficult one i was using so far)

4. Difficult part
```
```
 void calculateTip() {
 ```
    final totalAmount = double.parse(controller.text);
    final selectedIndex = isSelected.indexWhere((element) => element);
    final tipPercentage = [0.1, 0.2, 0.3][selectedIndex];
    final tipTotal = (totalAmount * tipPercentage).toStringAsFixed(2);
```
    setState(() {
      tip = '\$$tipTotal';
    });
  }
```
first we received our user-input value
then we used the list of booleans...
last we assigned empty tip to our result

