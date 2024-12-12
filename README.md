# JavaScript Loose Equality Bug

This repository demonstrates a common JavaScript bug related to loose equality (==) when handling null and undefined values.  The bug arises from the fact that `null == undefined` evaluates to `true`, while `null === undefined` evaluates to `false`.  This can lead to unexpected NaN results when performing arithmetic operations.

## Bug Description

The provided JavaScript code uses loose equality to check for null. However, when an undefined value is passed, it evaluates to NaN due to the loose comparison not accurately reflecting the intended null check.

## Solution

The solution involves using strict equality (===) to explicitly check for null and handle undefined values separately.