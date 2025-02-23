# Responsive Flexbox Layout Task

## 📌 Task 1: Improve the Flexbox Layout & Responsiveness

### **🎯 Goal:**
Modify your existing layout to make it **more flexible and better suited for various screen sizes** using **Flexbox**.

## 📋 Steps to Complete:

### **1️⃣ Enable Wrapping for Flex Items**
Prevent cards from shrinking too much by allowing them to wrap to the next row when necessary.
```css
.container {
  display: flex;
  flex-wrap: wrap; /* Allow items to wrap instead of shrinking too much */
  justify-content: center; /* Center align when wrapping */
}
```

### **2️⃣ Set a Dynamic Size for Cards**
Ensure the cards **shrink and grow** dynamically to fit the screen.
```css
.card {
  flex: 1 1 300px; /* Cards take at least 300px width and shrink if needed */
}
```

### **3️⃣ Adjust Layout for Smaller Screens**
Make the layout responsive for mobile devices by stacking the cards vertically.
```css
@media screen and (max-width: 768px) {
  .container {
    flex-direction: column;
    align-items: center;
  }
  
  .card {
    width: 90%; /* Make cards take most of the width on smaller screens */
  }
}
```

## ✅ Expected Behavior
- **Large screens**: Cards should stay in a row but wrap when necessary.
- **Medium screens (tablets)**: Cards should still be in a row but adjust dynamically.
- **Small screens (mobile)**: Cards should stack vertically.

## 🎯 Bonus Challenge:
- Add `gap: 20px;` in `.container` to create space between wrapped cards.
- Experiment with `justify-content` properties to see different alignment behaviors.

---
🚀 Once you complete this task, let me know, and I'll give you a slightly harder Flexbox challenge!