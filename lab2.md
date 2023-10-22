Part 1: 

For each of the two screenshots, describe:

'''

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

'''

Part 2:

Path to private key:

![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/720bb11a-7ddb-40f6-8e36-19a774794181)


Path to public key:

![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/ca2136da-f8ae-4280-b450-85fa2b2ad292)


Logging into ieng6 without password prompt:

![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/9a861a59-2d03-4657-bf9e-1277b33d6c94)


Part 3:

I learned that there's a lot of ways to interact with web related services and servers in the search bar that connect to the URL's I see when I search for videos on YouTube or Google, when I add or do different operations on websites like calculators, etc. and those update on the URL in ways that I would always see but would never think about. In addition, In labs 2 and 3 I've been able to finally connect the terminal work that we do to my own computer for example, and navigating remoting into different computers, working with making my own code/methods, etc. that makes me really connect the relevance of my coding experience to linux.
