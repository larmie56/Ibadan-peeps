# Ibadan-peeps
Regional mutism

/**in light of recent Lagos slander (especially by Ibadan peeps), 
it has become necessary to find a way to keep them mute. 
ladies and gentlemen, I present to you, 'Regional Mutism'. */

import java.util.Scanner;
import static java.lang.System.out;

public class IbadanPeeps {

static boolean fromIbadan, slandersLagos;
	
	 static void questionnaire() {
		 Scanner keyboard = new Scanner(System.in);
		 out.print("What do you have to say about Lagos? ");
			String answer = keyboard.nextLine();
			out.print("Are you from Ibadan? (true/false) ");
			fromIbadan = keyboard.nextBoolean();
			
			if (answer.contains("traffic"))
				slandersLagos = true;
			if (answer.contains("dirty"))
				slandersLagos = true;
	}
	
	static void keepingIbadanPeepsInCheck() {
		if (fromIbadan && slandersLagos) {
			out.println("For the sake of world peace, you've been muted. Now think about your actions.");
		}
		else if (!fromIbadan && slandersLagos) {
			out.println("Your location has saved you, go and sin no more.");
		}
		else {
			out.print("Such faith in Lagos has never been seen anywhere in the world. Go in peace, your faith has saved you.");
		}
	}
	
	public static void main(String[] args) {
		questionnaire();
		keepingIbadanPeepsInCheck();
	}

}
