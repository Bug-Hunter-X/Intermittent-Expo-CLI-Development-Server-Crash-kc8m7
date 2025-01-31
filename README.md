# Expo CLI Intermittent Crash Bug

This repository demonstrates a bug encountered with the Expo CLI where the development server would crash intermittently without providing any specific error messages. The crash is non-deterministic, making it difficult to pinpoint the cause.

## Bug Description

The Expo development server crashes unexpectedly during normal operation.  The Metro bundler terminates without providing useful error information to the console.  This occurs across different platforms (iOS, Android simulators and devices) and does not appear to be tied to any specific user action.

## Reproduction Steps

While there are no specific steps to reliably reproduce the bug, the issue manifested inconsistently throughout development.

1. Start the Expo development server using `expo start`.
2. Observe normal application operation for a variable amount of time.
3. The server will abruptly crash and restart, without any clear indication in the console about the cause.

## Potential Solutions (Investigative)

The proposed solution involves logging various aspects of the app's lifecycle and the environment to possibly find a correlation with the crashes.

## Additional Notes

The lack of error messages significantly impacts debugging efforts. This bug is non-deterministic and its root cause remains unidentified in this example. More information would be needed for definitive resolution.