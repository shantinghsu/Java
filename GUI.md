# Java GUI
### Set up the frame: JFrame class
`JFrame frame = new JFrame();`
1. Set size of frame (width & height)
```
  final int FRAME_WIDTH = 300;
  final int FRAME_HEIGHT = 400;
  frame.setSize(FRAME_WIDTH, FRAME_HEIGHT);
```
2. set title of frame (or omit this step to leave it blank)  
`frame.setTitle("An empty frame");`

3. Set "default close operation" to close the frame and EXIT the program  
`frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);`

4. Make the frame visible  
`frame.setVisible(true);`


### Adding User-Interface Components to a Frame:
`JPanel panel = new JPanel();`
`JButton button = new JButton("Words that display on the botton");`
`JLabel label = new JLabel("Words that display on the label")`
1. Set up the panel (default position at BorderLayout.CENTER in the frame)
  ```
  panel.add(botton);
  panel.add(label);
  ```
2. set up the frame with size, title, closure and visible


