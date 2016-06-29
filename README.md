# Day-13

import java.util.ArrayList;

public class CardDriver
{
   //-----------------------------------------------------------------
   //  Creates a deck, shuffles the deck and deals the cards.
   //-----------------------------------------------------------------
   public static void main (String args[])
   {
	  
	   ArrayList<Card> hand1 = new ArrayList<Card>(7);
	   ArrayList<Card> hand2 = new ArrayList<Card>(7);
	   
	   DeckOfCards gameDeck = new DeckOfCards();
	   
	   Card card1 = new Card();
	   Card card2 = new Card();
	  
	   gameDeck.shuffle();
	   
	   for ( int x = 0; x < 7; x++)
	   {
		   card1 = gameDeck.deal();
		   hand1.add(card1);
		   
		   card2 = gameDeck.deal();
		   hand2.add(card2);
	   }
	   
	   System.out.println("Player 1's Hand: ");
	   System.out.println("");
	   System.out.println(hand1);
	   
	   System.out.println("");
	   
	   System.out.println("Player 2's Hand: ");
	   System.out.println("");
	   System.out.println(hand2);       
       
       
   }
}
