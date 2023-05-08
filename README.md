# Flutter Stepper

A flutter package to create easily customizable Horizontal and Vertical stepper.

## Getting started

In the dependencies: section of your pubspec.yaml, add the following line:

   ```
   dependencies:
  another_stepper: <latest_version>
   ```

Import the following in your working dart file:

   ```
   import 'package:another_stepper/another_stepper.dart';
   ```

## Example AnotherStepper

### Dummy StepperData

   ```
   List<StepperData> stepperData = [
  StepperData(
      title: StepperText(
        "Order Placed",
        textStyle: const TextStyle(
          color: Colors.grey,
        ),
      ),
      subtitle: StepperText("Your order has been placed"),
      iconWidget: Container(
        padding: const EdgeInsets.all(8),
        decoration: const BoxDecoration(
            color: Colors.green,
            borderRadius: BorderRadius.all(Radius.circular(30))),
        child: const Icon(Icons.looks_one, color: Colors.white),
      )),
  StepperData(
      title: StepperText("Preparing"),
      subtitle: StepperText("Your order is being prepared"),
      iconWidget: Container(
        padding: const EdgeInsets.all(8),
        decoration: const BoxDecoration(
            color: Colors.green,
            borderRadius: BorderRadius.all(Radius.circular(30))),
        child: const Icon(Icons.looks_two, color: Colors.white),
      )),
  StepperData(
      title: StepperText("On the way"),
      subtitle: StepperText(
          "Our delivery executive is on the way to deliver your item"),
      iconWidget: Container(
        padding: const EdgeInsets.all(8),
        decoration: const BoxDecoration(
            color: Colors.green,
            borderRadius: BorderRadius.all(Radius.circular(30))),
        child: const Icon(Icons.looks_3, color: Colors.white),
      )),
  StepperData(
    title: StepperText("Delivered",
        textStyle: const TextStyle(
          color: Colors.grey,
        )),
  ),
];
```

### Dummy StepperText

   ```
   StepperText("Delivered",
        textStyle: const TextStyle(
          color: Colors.grey)),
   ```

### Horizontal(Default)

   ```
   AnotherStepper(
  stepperList: stepperData,
  stepperDirection: Axis.horizontal,
  iconWidth: 40, // Height that will be applied to all the stepper icons
  iconHeight: 40, // Width that will be applied to all the stepper icons
)
   ```

### Vertical(Default)

   ```
   AnotherStepper(
  stepperList: stepperData,
  stepperDirection: Axis.vertical,
  iconWidth: 40, // Height that will be applied to all the stepper icons
  iconHeight: 40, // Width that will be applied to all the stepper icons
)
```


