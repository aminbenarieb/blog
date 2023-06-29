---
title: "How to debug iOS web with local server"
date: 2023-06-29T14:27:48+01:00
---

```swift
private func send(
        peripheral: CBPeripheral?,
        characteristic: CBCharacteristic?,
        data: Data
    ) throws {
        guard
            let peripheral = peripheral,
            let characteristic = characteristic
        else {
            throw CellyError(
                message: "Trying to send data before discovring peripheral with characteristic",
                status: -1
            )
        }
        peripheral.writeValue(data, for: characteristic, type: .withoutResponse)
    }
```

and

```python
print("Hello World!")
```

