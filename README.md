# problemsolving-ballons-and-arrows
class Main {
    public static void main(String[] args) {
      int[][] ballons= {{1,6} ,{2,8},{7,12},{10,6}};
      int arrows = 1;
      int currentend = ballons[0][1];
      for(int i=0;i<ballons.length;i++){
          if(ballons[i][0]>currentend){
              arrows++;
              currentend = ballons[i][1];
          }
        }
        System.out.println(arrows);
      }
}
