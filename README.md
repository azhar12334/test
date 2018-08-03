# test
//
//  creatViewController.swift
//  hamalti
//
//  Created by program on 8/2/18.
//  Copyright © 2018 program. All rights reserved.
//
import UIKit

class creatViewController: UIViewController {

    @IBOutlet weak var creatprofile: UIButton!
    
    
    override func viewDidLoad() {
        super.viewDidLoad()

        // Do any additional setup after loading the view.
    }

    override func didReceiveMemoryWarning() {
        super.didReceiveMemoryWarning()
        // Dispose of any resources that can be recreated.
    }
    
    @IBAction func creat(_ sender: UIButton)
    {
        
        func creteAlter (title : String, message : String)
        {
            let alert = UIAlertController(title: title, message: message, preferredStyle: UIAlertControllerStyle.alert)
            
            alert.addAction(UIAlertAction(title: "ok", style: UIAlertActionStyle.default, handler: {(action ) in
                
                alert.dismiss(animated: true, completion: nil) } ))
            
            self.present(alert,animated: true , completion: nil)
            
        }//end of fucntion
       
    }
    
//    override func viewDidAppear(_ animated: Bool)
//    {
//        creteAlter(title: "Verification", message: "Please confirm your email address")
//        
//    }//end
    
    /*
    // MARK: - Navigation
    // In a storyboard-based application, you will often want to do a little preparation before navigation
    override func prepare(for segue: UIStoryboardSegue, sender: Any?) {
        // Get the new view controller using segue.destinationViewController.
        // Pass the selected object to the new view controller.
    }
    */

}
