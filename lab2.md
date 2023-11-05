Part 1: 

First SC Of Bot Working:

![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/69883145-fbee-49aa-98da-62d8c2c71abf)

In this screenshot, handleRequest and main methods are called.

Main takes in a String parameter that is labelled as args, which has the value of the port number. HandleRequest takes in a URI parameter called URL, taking in the URL of the path. add-message is the parameter searched for by the if statement, and in the URL itself, and the port number of 4000 that I used is in the beginning of the URL, as it was taken in earlier.

From this specific request, words value is changed to "SC Works", count changes from 2 to 3, noPlus is set to "" (blank).

Second SC of Bot Working:

![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/aa4dd1dc-7c60-4b7d-95f0-dab8685f15ea)

In this screenshot, handleRequest and main methods are called.

Main takes in a String parameter that is labelled as args, which has the value of the port number. HandleRequest takes in a URI parameter called URL, taking in the URL of the path. add-message is the parameter searched for by the if statement, and in the URL itself, and the port number of 4000 that I used is in the beginning of the URL, as it was taken in earlier.

Count and strCount changes from 3 to 4, words becomes "SC+Works", and NoPlus becomes "SC Works".

StringServer:

```

import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    String words = "";
    int count = 0;
    String strCount = "";

    public String handleRequest(URI url) {
            String noPlus = "";
        if (url.getPath().equals("/")) {
            return String.format(words);
        } else {
            if (url.getPath().contains("/add-message")) {
                String[] parameters = url.getQuery().split("=");
                if (parameters[0].equals("s")) {
                    count += 1;
                    strCount = Integer.toString(count);
                    words += strCount + ". " + parameters[1] + "\n";

                    for (int i = 0; i < words.length(); i++) {
                        if (words.charAt(i) != '+') {
                            noPlus += words.charAt(i);
                        } else {
                            noPlus += " ";
                        }
                    }
                            return noPlus;

                }
            }
            return "404 Not Found!";
        }
    }
}

class StringServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}

```

Part 2:

Path to private key:

<img width="353" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/89326458-e37d-4315-9049-9db1fc1901b9">


Path to public key:

<img width="571" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/b9c21e57-0ece-4ada-86db-0c6467db6fb5">


Logging into ieng6 without password prompt:


![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/f9db8a4f-1a08-4a06-abc5-e131a996d090)



Part 3:

I learned that there's a lot of ways to interact with web related services and servers in the search bar that connect to the URL's I see when I search for videos on YouTube or Google, when I add or do different operations on websites like calculators, etc. and those update on the URL in ways that I would always see but would never think about. In addition, In labs 2 and 3 I've been able to finally connect the terminal work that we do to my own computer for example, and navigating remoting into different computers, working with making my own code/methods, etc. that makes me really connect the relevance of my coding experience to linux.
