# CallKit
A nice wrapper over iOS CallKit Framework.

How to use:
- Setup once

  [[ADCallKitManager sharedInstance] setupWithAppName:@"Bolo" supportsVideo:YES actionNotificationBlock:^(CXCallAction * _Nonnull action, ADCallActionType actionType) {
        }];
        
- Report Incoming Call

  NSUUID *callUUID = [[ADCallKitManager sharedInstance] reportIncomingCallWithContact:ontact completion:^(NSError * _Nullable error) {
    }];
    
- Report Outgoing Call

  NSUUID *callUUID = [[ADCallKitManager sharedInstance] reportOutgoingCallWithContact:contact completion:^(NSError * _Nullable error) {
    }];
    
  
