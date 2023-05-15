## // 1. Array codes anlegen
	````Java
    public class RotiereArray {

	public static void main(String[] args) {
		// 1. Array codes anlegen
		int[][] codes =getCodes(3);
		
		// 2. codes ausgeben
		ausgabe(codes);
		
		// 3. codes rotieren
		int[][] rotierteCodes = rotateRight(codes);

		// 4. rotierte Codes ausgeben
		ausgabe(rotierteCodes);

	}

	private static int[][] getCodes(int dimension) { //1.
		int[][] c = new int[dimension][dimension];

		int wert = 1;

		for (int y = 0; y < c.length; y++) {
			for (int x = 0; x < c.length; x++) {
				c[y][x] = wert;
				wert++;
			}
		}

		return c;
	}

	
	private static void ausgabe(int[][] codes) { //2.

		for (int y = 0; y < codes.length; y++) {
			for (int x = 0; x < codes.length; x++) {
				System.out.print(codes[y][x] + "\t");
			}
			System.out.println();
		}
		System.out.println("----------------------------------------");

	
	}	
	

    private static int[][] rotateRight(int[][] codes) {//3.
    	
    	int[][] c = new int [codes.length][codes.length];
    	
    	for (int y = 0; y < codes.length; y++) {
    		for (int x = 0; x < codes.length; x++) {
    			c[y][x]=codes[codes.length-1-x][y];
				
			}
    	}
    	return c;
    	
    }

}
    