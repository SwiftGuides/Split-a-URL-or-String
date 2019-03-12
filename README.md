# Split-a-URL-or-String
Guide to Split URL to get only needed Values from the whole URL


                    let fileName = "rtmp://a51abd.entrypoint.cloud.wowza.com/app-2240"
                    
                    //Split the String on behalf of "//"
                    let filearray2 = fileName.components(separatedBy: "//")
                    
                    //Gets the String After "//"
                    let finalFileName = filearray2.last
                    
                    //Split the String on behalf of "/"
                    let FinalString = finalFileName?.components(separatedBy: "/")
                    
                    // Get String Value before "/" Charset
                    let hostAddress = FinalString?.first
                    
                    //Get String Value After "/" Charset
                    let applicationName = FinalString?.last
