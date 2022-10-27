# fix_most_flutter_errors



These commands will solve many issues that you face when running a flutter app on an IOS device. It will also free some space by deleting the derived data in your xCode folder.

NB: I tested with android and it worked!

Make sure you are in the root of your Flutter project and copy and paste these following codes in your terminal:




- flutter clean 
- rm -Rf ios/Pods 
- rm -Rf ios/.symlinks 
- rm -Rf ios/Flutter/Flutter.framework 
- rm -Rf Flutter/Flutter.podspec 
- rm ios/podfile.lock 
- cd ios 
- pod deintegrate 
- sudo rm -rf ~/Library/Developer/Xcode/DerivedData 
- flutter pub cache repair 
- flutter pub get 
- flutter pub upgrade 
- flutter pub upgrade --major-versions 
- Pod update 
- pod install 
- flutter run
