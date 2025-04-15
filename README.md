# Practical-no.-7

## **Practical 7: Modeling Sequence Diagrams**  
**Topic:** Ayurvedic Management System  
**Objective:**  
To model the interaction between various objects in the Ayurvedic Management System using a sequence diagram, showing the flow of messages and the order of operations.

---

### **Sequence Diagram**  
A sequence diagram is a type of interaction diagram that shows how objects operate with one another and in what order. It illustrates the sequence of messages exchanged between the objects to carry out the functionality of a particular use case.

---

### **Elements in Sequence Diagram:**
- **Objects (Participants):** Represented by rectangles with object names underlined.  
  *Examples:* Patient, Receptionist, Doctor, Inventory System, Billing System.
  
- **Lifeline Bars:** Dotted vertical lines that represent the existence of an object over time.

- **Activation Bars:** Thin rectangles on lifelines showing the duration of execution of a process.

- **Messages:** Arrows that show communication between objects.
  - **Synchronous Messages:** Represent a call that waits for a response.
  - **Asynchronous Messages:** Represent a call that does not wait for a response.

---

### **Example (Ayurvedic Management System Use Case – Book Appointment & Generate Bill):**

**Objects Involved:**  
Patient → Receptionist → Doctor → Inventory System → Billing System

**Flow:**
1. **Patient → Receptionist:** Request for appointment  
2. **Receptionist → Doctor:** Check availability  
3. **Doctor → Receptionist:** Confirms slot  
4. **Receptionist → Patient:** Confirms appointment  
5. **Doctor → Inventory System:** Checks for available medicines  
6. **Inventory System → Doctor:** Sends availability  
7. **Doctor → Billing System:** Sends prescription for billing  
8. **Billing System → Patient:** Generates and sends bill

---

### **Synchronous Messages:**  
- Patient requesting appointment from Receptionist  
- Receptionist checking availability with Doctor  
- Doctor accessing Inventory System

### **Asynchronous Messages:**  
- Notifications sent from Billing System to Patient  
- Alerts sent from Inventory to Admin if stock is low

![image](https://github.com/user-attachments/assets/a68f9b8c-66af-4ef0-b4b1-fb253c9fcd68)

![17446904086328450501393065156755](https://github.com/user-attachments/assets/30438427-cb27-4a24-94cf-f8e03cdbd73d)
