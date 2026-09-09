## Cael Meacham
My favorite city to visit is Seattle Washington. I have been there twice in the last 3 years and have enjoyed it very much. To get there, my family would take an hour long ferry ride which is very fun because you get to see some beautiful scenery as well as some extremely nice houses. And the city has a lot of different places to visit and shop at.

[Seattle]("Seattle-background-Mount-Rainier.webp")

---
## New Cities to Visit
I am creating a table for the new cities I would like to visit in my future. The table will contain the name of the city, the reason I want to visit, how far it is from my favorite city, and how much it would cost to visit there.

| Cities to Visit | Reason | Distance | Cost |
| --- | --- | --- | --- |
| Athens | Old Architecture, Beautiful landscape, Historical significance | 6,200 miles | $712-$1,054 |
| New York City | Walk through times square during Christmas time | 2,420 miles | $220-$480 |
| Los Angeles | Great weather and the Hollywood walk of fame | 954 miles | $130-$310 |
| Miami | Hangout at the beach and golf along the east coast | 2,724 miles | $220-$450 |

---

## Jokes
> Jake: What did the ocean say to the beach? Nothing, it just waved.

> Henry: Dogs can't operate MRI machinery, but catscan

---
## Code Fencing
The snippet that I got based on my 919# is "Connecting to and reading from a web page. the purpose of this snippet is to be able to open a site on a web browser, read the text in the site, and copy the text in that site into a new file on your computer.

~~~
import java.io.InputStreamReader;
import java.net.URL;
import java.net.URLConnection;
import java.util.Scanner;


public class URLExpSimple {

    
    public static void main(String[] args) {
        try {
            URL mySite = new URL("http://www.cs.utexas.edu/~scottm");
            URLConnection yc = mySite.openConnection();
            Scanner in = new Scanner(new InputStreamReader(yc.getInputStream()));
            int count = 0;
            while (in.hasNext()) {
                System.out.println(in.next());
                count++;
            }
            System.out.println("Number of tokens: " + count);
            in.close();
        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}
~~~

[Link to snippet](https://www.cs.utexas.edu/~scottm/cs307/javacode/codeSamples/URLExpSimple.java)