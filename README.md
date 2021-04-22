# autocomplete_textfield_ns

An autocomplete textfield for flutter

## Pull requests

Feel free to submit pull requests for desired changes / features / bug fixes... It makes the maintenance of this code much easier.

## Usage

AutoCompleteTextField supports any data type suggestions
 `AutoCompleteTextField<YOURDATATYPE>()`  
The suggestions parameter must have data that matches `<YOURDATATYPE>`  
A global key of type `GlobalKey<AutoCompleteTextFieldState<T>>` is required so that the `clear()` method can be called to clear AutoCompleteTextField.

## Strings and itemFilter

Filtering is case sensitive so when using strings a common implementation of itemFilter is .

```dart
itemFilter: (item, query) {
  return item.toLowerCase().startsWith(query.toLowerCase());
}
```

![Textfield Demo](textfield-demo.gif)
