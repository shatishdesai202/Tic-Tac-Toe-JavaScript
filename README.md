# Tic-Tac-Toe-JavaScript



Game -Functionality :
    --> Score Reset
    --> Game Reset


    Proporty(CSS) Used :
        `.style.pointerEvents = 'none'`
        `.style.pointerEvents = 'auto'`
        
        Game Logic
        
function winner() {
    if (check(1, 2, 3, sign) || check(4, 5, 6, sign) || check(7, 8, 9, sign) || check(1, 5, 9, sign) || check(3, 5, 7, sign) || check(1, 4, 7, sign) || check(2, 5, 8, sign) || check(3, 6, 9, sign)) {
        dis()
        document.getElementById('message').innerText = `${sign} Winner`
        if (sign == 'X') {
            scoreX++
        } else {
            scoreO++
        }
        document.getElementById('scoreo').innerText = scoreO
        document.getElementById('scorex').innerText = scoreX

        return true
    }
    else{
        if(getbox(1)!=""&& getbox(2)!=""&& getbox(3)!=""&&
       getbox(4)!=""&& getbox(5)!=""&& getbox(6)!=""&&
       getbox(7)!=""&& getbox(8)!=""&& getbox(9)!=""){
    
        document.getElementById('message').innerText = 'draw'
       }

}
