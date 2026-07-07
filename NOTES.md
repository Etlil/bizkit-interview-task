I focused on Bug #1 first since it was the original issue. At first I couldn't find the double-booking bug, but after testing more, I found it: when I booked a range that surrounded an existing booking, it still let the booking go through. Since I wasn't familiar with the code yet, I gave it to AI to find the exact line causing the problem, and it suggested the fix.

Existing booking: Jan 10–15. New booking: Jan 9–16, the original code allowed this (wrongly), the fix now blocks it.

I used AI to help analyze the code and pinpoint where the bug was, and before committing, I tested the fix myself to confirm it actually worked.