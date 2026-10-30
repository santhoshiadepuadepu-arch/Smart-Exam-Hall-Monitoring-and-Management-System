# Smart Exam Hall Monitoring and Management System

## 📌 Project Overview
The Smart Exam Hall Monitoring and Management System is an LPC2148-based embedded system designed to automate examination timing, monitor room temperature, and provide visual and audio alerts. It helps invigilators manage examination activities efficiently, reduce manual timing errors, and improve examination hall management.

## 🎯 Objectives
- Display current RTC time and room temperature on a 16×2 LCD.
- Configure examination duration using a 4×4 matrix keypad.
- Implement a countdown timer for examination management.
- Display remaining examination time using two multiplexed 7-segment displays.
- Provide Green, Yellow, and Red LED alerts based on remaining time.
- Enable password-protected RTC and examination configuration.
- Implement Pause/Resume functionality using external interrupts.
- Monitor room temperature using an LM35 sensor.
- Automatically record examination start and end times.

## ⚙️ Hardware Requirements
- LPC2148 Microcontroller
- 16×2 LCD
- 4×4 Matrix Keypad
- Switches
- Two 7-Segment Displays
- LM35 Temperature Sensor
- LEDs (Green, Yellow, Red)
- Buzzer
- USB-UART Converter / DB-9 Cable

## 💻 Software Requirements
- Embedded C Programming
- Keil µVision
- Flash Magic
- Proteus (for simulation, if used)

##Block Diagram

<img width="720" height="571" alt="WhatsApp Image 2026-10-30 at 8 28 20 PM" src="https://github.com/user-attachments/assets/e455d787-7cb4-41a3-ba32-e3f5f43abcec" />


## 🔄 Working Principle

1. **Normal Monitoring:** The LCD displays the current date, time, and room temperature.
2. **Configuration:** The invigilator presses Switch-1 (External Interrupt 0) and enters the admin password using the keypad.
3. **Examination Setup:** After successful authentication, the invigilator can configure RTC date, time, examination start time, and duration.
4. **Countdown Timer:** Once the examination starts, the system records the start time and begins the countdown.
5. **Time Display:** The remaining examination time is displayed on two multiplexed 7-segment displays.
6. **LED Indication:**
   - Green LED: More than 10 minutes remaining.
   - Yellow LED: Final 10 minutes.
   - Red LED: Final 1 minute.
7. **Buzzer Alert:** The buzzer activates when the countdown reaches zero.
8. **Temperature Monitoring:** The LM35 sensor continuously measures room temperature, which is displayed on the LCD.
9. **Pause/Resume:** Switch-2 (External Interrupt 1) pauses and resumes the countdown timer.
10. **Automatic Logging:** Examination start and end times are recorded using the RTC.

## ⭐ Key Features
- Automated examination timing.
- Password-protected configuration.
- Real-time temperature monitoring.
- Countdown timer management.
- LED-based examination status indication.
- Buzzer notification at examination completion.
- Pause and Resume functionality.
- Automatic recording of examination start and end times.

## 📈 Benefits
- Reduces manual timing errors.
- Improves examination management efficiency.
- Provides clear examination status indications.
- Helps invigilators monitor time and room temperature.
- Offers a reliable and cost-effective embedded solution.

## 🏁 Conclusion
The Smart Exam Hall Monitoring and Management System provides an automated approach to examination hall management by combining RTC-based timekeeping, countdown management, temperature monitoring, interrupt-driven control, and automatic event logging.

## 👩‍💻 Technologies Used
- Embedded C
- ARM7 (LPC2148)
- Microcontroller Interfacing
- RTC
- LCD and Keypad Interfacing
- LM35 Sensor
- Interrupt Programming
- 7-Segment Display Interfacing

---
**Project Name:** Smart Exam Hall Monitoring and Management System  
**Controller:** LPC2148  
**Domain:** Embedded Systems
