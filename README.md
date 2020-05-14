# GAME
public class UZAYOYUNU extends JFrame{
  private UZAYOYUNU(String space_game) {
      super(space_game);
  }
    public static void main(String[] args) {
        UZAYOYUNU game = new UZAYOYUNU("SPACE GAME");
        
        game.setResizable(false);
        game.setFocusable(false);
        game.setSize(800,600);
        game.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        
        UZAYARKA panel = new UZAYARKA();
        panel.requestFocus();
        panel.addKeyListener(panel);
        panel.setFocusable(true);
        panel.setFocusTraversalKeysEnabled(false);
        game.add(panel);
        game.setLocation(400,100);
        
        
        game.setVisible(true);
        
        
    }

  
    }
