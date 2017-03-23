# Quick Storage Framework

An objective-C iOS framework that stores things like an dictionary

## Installation

Copy the files to the project file

## How to Use

### Import

```objective-c
import "QuickStorage.h"
```

### Store

```objective-c
NSString *obj1 = @"Fdis";
NSDictionary *obj2 = [@"Key": [@"Data1", @"Data2"]];
[QuickStorage storeObject:obj1 forKey:@"SomeKey"];
[QuickStorage storeObject:obj2 forKey:@"SomeOtherKey"];
```

### Retrive

```objective-c
NSString *str = [QuickStorage objectForKey:@"SomeKey"];
NSArray *arr = [QuickStorage objectForKey:@"SomeOtherKey"];
```

### Check

```objective-c
BOOL exists = [QuickStorage isObjectStoredWithKey:@"SomeKey"]; // ture, YES
BOOL exists = [QuickStorage isObjectStoredWithKey:@"SXXX"]; // false, NO
```

### Delete

```objective-c
[QuickStorage deleteObjectForKey:@"SomeKey"];
```


### Savings

No Extra Work, QuickStorage auto saves.

## License

You are freely to edit, redistribute, etc. You can do anything with it. Perhaps Apache?
