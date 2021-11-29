import java.io.*;
public class Main
{
    
    public static void main(String[] args)
    {
        try{

File file=new File("/storage/emulated/0/File_exemple");
    file.mkdir();
        
    FileWriter fw=new FileWriter("/storage/emulated/0/File_exemple/file.txt");
    
       fw.write("Hello guys !!!");
   
       fw.close();
        
        FileReader fr=new FileReader("/storage/emulated/0/File_exemple/file.txt");
            
            int c;
            while((c=fr.read())!=-1){
                System.out.print((char) c);
            }
            fr.close();
            
        file.Delate();
            
            
            
        }
        catch(Exception e){
            e.printStackTrace();
        }
        
        
        
    }
    
        
}
