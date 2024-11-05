---
sticker: emoji//1f9b9-200d-2640-fe0f
tags:
  - dart
  - dev
  - basic_functionality
---

### Async

```
import 'dart:async';

Future<String> fetchData() async {
  // Simulating a network call with a 2-second delay
  await Future.delayed(Duration(seconds: 2));
  return 'Data received';
}

void main() async {
  print('Fetching data...');
  String data = await fetchData(); // Waits for fetchData to complete
  print(data);
}

```

`Future` → like promises in JavaScript (it can be completed or incompleted)
`await` → wait for response
`async` → call an async function