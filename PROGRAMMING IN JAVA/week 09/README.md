# Programming In Java WEEK 09
#### 1.**Which Swing component is best suited for displaying a drop-down list of selectable options?**

a. JButton  
b. JComboBox  
c. JTextField  
d. JPanel  

**Answer:** b. JComboBox

---
#### 2. **What will be the output of the following Java code?**

```java
import javax.swing.*;
import java.awt.*;

public class SwingExample {
    public static void main(String[] args) {
        JFrame frame = new JFrame("Example");
        frame.setLayout(new FlowLayout());
        frame.add(new JButton("Button 1"));
        frame.add(new JButton("Button 2"));
        frame.setSize(300, 200);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.setVisible(true);
    }
}
```

**a.** A frame with two buttons labeled “Button 1” and “Button 2”.  
**b.** A frame with only one button labeled “Button 2”.  
**c.** Compilation Error.  
**d.** Runtime Error.  

**Answer:** a. A frame with two buttons labeled “Button 1” and “Button 2”.

---

#### 3. **Which of the following is true about the `JLabel` component in Java Swing?**

a. It is used only for displaying text.  
b. It can display text and icons.  
c. It cannot be added to a `JPanel`.  
d. It generates mouse events by default.  

**Answer:** b. It can display text and icons.

---

#### 4. **Which method is used to handle mouse click events in Java Swing?**

a. `mouseClicked()`  
b. `keyPressed()`  
c. `actionPerformed()`  
d. `componentShown()`  

**Answer:** a. `mouseClicked()`

---

#### 5. **What should replace `// INSERT CODE HERE` to create a `JFrame` with a `JButton` labeled "Click Me"?**

```java
import javax.swing.*;

public class FrameExample {
    public static void main(String[] args) {
        JFrame frame = new JFrame("Demo Frame");
        JButton button = new JButton("Click Me");
        // INSERT CODE HERE
        frame.setSize(300, 200);
        frame.setVisible(true);
    }
}
```

a. `frame.add(button);`  
b. `frame.insert(button);`  
c. `frame.append(button);`  
d. `frame.push(button);`  

**Answer:** a. `frame.add(button);`

---

#### 6. **Identify and correct the error in the following program:**

```
import javax.swing.*;
import java.awt.*;

public class PanelExample {
    public static void main(String[] args) {
        JFrame frame = new JFrame("Panel Example");
        JPanel panel = new JPanel();
        JButton button = new JButton("Submit");
        panel.setFlowLayout(); // ERROR
        panel.add(button);
        frame.add(panel);
        frame.setSize(300, 200);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.setVisible(true);
    }
}
```

**What should the erroneous line (`panel.setFlowLayout();`) be replaced with?**

a. `panel.setLayout(new GridLayout());`  
b. `panel.addFlowLayout();`  
c. `panel.appendLayout(new FlowLayout());`  
d. `panel.setLayout(new FlowLayout());`  

---

**answer:**  
d. `panel.setLayout(new FlowLayout());`

---

#### 7. **What will the following Java program output?**

```java
import javax.swing.*;

public class LabelExample {
    public static void main(String[] args) {
        JFrame frame = new JFrame("Label Demo");
        JLabel label = new JLabel("Welcome to Swing");
        frame.setSize(250, 100);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.setVisible(true);
    }
}
```

**a.** A frame with the label "Welcome to Swing".  
**b.** A frame with no visible label.  
**c.** Compilation Error.  
**d.** Runtime Error.  

**Answer:**  
b. A frame with no visible label.

---

#### 8. **What does the following code do?**

```java
import javax.swing.*;

public class NPTEL extends JFrame {
    JButton button;

    public NPTEL() {
        button = new JButton("Programming in Java");
        add(button);
        setSize(300, 200);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setVisible(true);
    }

    public static void main(String[] args) {
        new NPTEL();
    }
}
```

**a.** Creates a JFrame with a JButton labeled "Programming in Java"  
**b.** Compiles with errors  
**c.** Displays a message dialog  
**d.** Creates a JPanel with a JButton labeled "Programming in Java"  

**Answer:**  
**a. Creates a JFrame with a JButton labeled "Programming in Java"**

---

#### 9. **What happens when the button in this Java code snippet is clicked?**

```java
import javax.swing.*;
import java.awt.event.*;
public class NPTEL {
    public static void main(String[] args) {
        JFrame frame = new JFrame("NPTEL Java Course");
        JButton button = new JButton("Click Me!");
        button.setBounds(50, 100, 100, 40);
        button.addActionListener(new ActionListener() {
            public void actionPerformed(ActionEvent e) {
                JOptionPane.showMessageDialog(null, "Welcome to the course");
            }
        });
        frame.add(button);
        frame.setSize(300, 200);
        frame.setLayout(null);
        frame.setVisible(true);
    }
}
```

**a.** The program exits  
**b.** A message dialog with the text "Welcome to the course" is displayed  
**c.** The button label changes to "Welcome to the course"  
**d.** Nothing happens  

**Answer:**  
**b. A message dialog with the text "Welcome to the course" is displayed**

---

#### 10. **The container displays a number of components in a column, with extra space going between the first two components.**

**Which of the following layout manager(s) most naturally suited for the described layout?**

**a.** BoxLayout  
**b.** FlowLayout  
**c.** BorderLayout  
**d.** GridLayout  

**Answer:**  
**a. BoxLayout**

---
