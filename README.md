import java.io.BufferedInputStream;
import java.io.FileInputStream;
import java.io.IOException;

public class Jala {
	public static void main(String[] args) throws IOException { 
  FileInputStream fis = new FileInputStream("myfile.txt");
        BufferedInputStream bis = new BufferedInputStream(fis);
        while(bis.available()!=0)
        {
        	System.out.println((char)bis.read());
        }
