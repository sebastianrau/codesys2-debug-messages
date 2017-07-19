# Codesys2-DebugMessages
Adding Debug Messaged to an Global Array

Usage:
- include Library
- (optinal) write the actucal time to <code>stDebugInformation.dtActualTime := SOME_TIME_VALRIABLE_AS_DT;</code>

- call function <code>DebugLog(...)</code> to add a Message to the Ringbuffer.  Parameters are:
```
sMessage 	: STRING(64);
ePriority 	: E_DebugMessagePriority;
```

- Prioritys are
```	
DEBUG := 0
INFO := 1
WARN := 2
ERROR := 3
FATAL := 4
```

- All Messaged will be added to the <code> stDebugInformation </code> Struct in Global Variables of the Lib
- Change the Ringbuffer size set the the <code> iMaxDebugEntries</code> constant in your project GVL.

