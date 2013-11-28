NSArray+SafeAccess
=========

When accessing an item from a NSArray object with an index out of the bounds of the NSArray, nil is returned instead of throwing a NSRangeException.

## Installation
Install via cocoapods by adding this to your Podfile:

	pod "NSArray+SafeAccess", "~> 0.0.1"

## Usage

Import header file:

	#import "NSArray+SafeAccess.h"
	
Access items of a NSArray object:

	NSArray *myArray = @[@"A", @"B", @"C"];
	NSString *myString = [myArray objectAtIndexOrNil:3]; // returns nil
