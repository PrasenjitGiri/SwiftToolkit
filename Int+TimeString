/* Swift extension to convert milliseconds to time string hh:mm:ss */

import Foundation

extension Int {
    
    func millisecondsToTimeString()-> String {
        
        let hours = self / (1000 * 60 * 60)
        let minutes = (self % (1000*60*60)) / (1000 * 60)
        let seconds = ((self % (1000*60*60)) % (1000*60)) / 1000
        
        let formatter = NSNumberFormatter()
        formatter.minimumIntegerDigits = 2
        
        let hoursString = formatter.stringFromNumber(hours)
        let minutesString = formatter.stringFromNumber(minutes)
        let secondsString = formatter.stringFromNumber(seconds)
        
        var timeString = String()
        timeString = "\(hoursString!):\(minutesString!):\(secondsString!)"
        return timeString
    }
}
