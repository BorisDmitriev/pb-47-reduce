# Array Methode .reduce
 Nehmen wir an, wir haben ein Array mit Benutzern in der Form `[{id:..., name:..., age:... }]` erhalten.

* Schau dir die Datei `index.js` an, sie enthält die Funktion `groupById`.
* Ergänze die Funktion `groupById` so, dass sie ein Objekt aus dem übergebenen Array erstellt und zurückgibt.
* Die Eigenschaftsnamen der neu erstellten Objekte sollten aus der ID jedes Objekts im Array id als Schlüssel erstellt werden.
* Die Werte der Eigenschaften sollten die jeweiligen Objekte aus dem Array sein.

## Beispiel:
```js
let users = [
  {id: 'john', name: "John Smith", age: 20},
  {id: 'ann', name: "Ann Smith", age: 24},
  {id: 'pete', name: "Pete Peterson", age: 31},
];

let usersById = groupById(users);

console.log(usersById)

/* erwartete Ausgabe:
{
  john: {id: 'john', name: "John Smith", age: 20},
  ann: {id: 'ann', name: "Ann Smith", age: 24},
  pete: {id: 'pete', name: "Pete Peterson", age: 31},
}
*/
```
* Eine solche Funktion ist sehr praktisch, wenn du mit Serverdaten arbeitest.

* In dieser Aufgabe gehen wir davon aus, dass id eindeutig ist. Es darf keine zwei Array-Elemente mit der gleichen id geben.

* Bitte verwende die Methode array.reduce in der Lösung.
