# Digital Watch-Clock - Assembly Language Project

## Project Description
This project demonstrates the implementation of a digital clock using assembly language and the Irvine32 library. The clock displays the current time (hours, minutes, and seconds) on a text-based console screen in HH:MM:SS format using 7-segment-like patterns. The clock updates every second and automatically refreshes the display.

## Group Members
- Dania Khan (23K-0072)
- Zunaira Amjad (23K-0013)

## Features
- Displays time in 7-segment style using ASCII characters
- Automatically updates every second
- Efficient time tracking with minimal CPU usage
- Clean console display with light cyan text on black background
- Uses Windows API (`GetLocalTime`) for accurate timekeeping

## Technical Implementation
### Data Section
- **Time Variables**: Stores hours, minutes, seconds, and tracks second changes
- **Digit Patterns**: 7x8 grid ASCII representations for digits 0-9
- **Display Parameters**: Specifies digit dimensions and pointers to patterns

### Code Structure
1. **Main Procedure**:
   - Retrieves system time using `GetLocalTime`
   - Checks for second changes
   - Clears screen and sets text color
   - Displays time in HH:MM:SS format
   - Implements 50ms delay to reduce CPU usage

2. **Display Functions**:
   - `DisplayDigit`: Shows digits using predefined patterns
   - `DisplayColon`: Displays the colon separator

3. **Helper Procedures**:
   - `Clrscr`: Clears console screen
   - `SetTextColor`: Configures display colors
   - `Gotoxy`: Positions cursor
   - `Delay`: Implements timing control

## Key Algorithms
- **Time Handling**: Uses system time API with second-change detection
- **Digit Display**: Prints character patterns row-by-row
- **CPU Optimization**: Implements controlled delays to reduce resource usage

## Learning Outcomes
This project provides practical experience with:
- Assembly language programming
- Low-level screen manipulation
- System time retrieval
- Console output management
- Efficient programming techniques

## Requirements
- MASM assembler
- Irvine32 library
- Windows operating system

## How to Run
1. Assemble the program using MASM
2. Link with Irvine32 library
3. Execute the resulting binary
4. The digital clock will appear in the console window

## Conclusion
This assembly language program effectively demonstrates fundamental concepts of low-level programming, including system calls, screen manipulation, and time management. It serves as an excellent foundation for understanding hardware-related programming tasks.
