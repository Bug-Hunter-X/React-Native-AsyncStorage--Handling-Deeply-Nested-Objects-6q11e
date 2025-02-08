# React Native AsyncStorage: Handling Deeply Nested Objects

This repository demonstrates a common issue and its solution when working with AsyncStorage in React Native and deeply nested objects. Directly storing complex objects in AsyncStorage can cause unpredictable behavior, such as data corruption or type mismatches. This example shows how to use JSON.stringify and JSON.parse to properly serialize and deserialize the data before and after storage.

## Problem

Attempting to store and retrieve deeply nested objects in AsyncStorage directly without proper serialization can result in data loss or unexpected data types.

## Solution

The solution involves converting the object into a JSON string before storing it in AsyncStorage and parsing the JSON string back into an object after retrieval.

## Setup

1. Clone the repository.
2. Navigate to the project directory in your terminal.
3. Run `npm install` to install dependencies.
4. Run the app using `npx react-native run-android` or `npx react-native run-ios`.

## Usage

The example includes two components: one to store the nested object and another to retrieve it.   Observe the console logs to understand the behavior with and without proper JSON serialization.