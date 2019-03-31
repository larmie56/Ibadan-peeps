# Ibadan-peeps
Regional mutism

/**in light of recent Lagos slander (especially by Ibadan peeps), 
it has become necessary to find a way to keep them mute. 
ladies and gentlemen, I present to you, 'Regional Mutism'. */

import java.util.Scanner;

public class IbadanPeeps {

	static Scanner keyboard;
	public static void main(String[] args) {
		
		keepingIbadanPeepsQuiet();
	}

	private static void keepingIbadanPeepsQuiet() {
		if (fromIbadan() && slanderLagos()) {
			System.out.println("For the sake of world peace, you've been muted. Now think about your actions.");
		}
		
		else {
			System.out.println("Your location and/or faith in Lagos has made you whole. Go in peace.");
		}
	}
	
	private static boolean fromIbadan() {
		keyboard = new Scanner(System.in);
		System.out.print("Are you from Ibadan? (true/false) ");
		boolean answer = keyboard.nextBoolean();
		
		return answer;
	}
	
	private static boolean slanderLagos() {
		keyboard = new Scanner(System.in);
		boolean answer;
		
		System.out.println("In one sentence, what do you have to say about Lagos? ");
		String reply = keyboard.nextLine();
		
		if (reply.contains("traffic") || reply.contains("dirty")) {
			answer = true;
		}
		else {
			answer = false;
		}
		
		return answer;
	}
}
