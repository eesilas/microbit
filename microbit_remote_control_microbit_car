function L () {
    SuperBit.MotorRunDual(
    SuperBit.enMotors.M1,
    n,
    SuperBit.enMotors.M2,
    p
    )
    SuperBit.MotorRunDual(
    SuperBit.enMotors.M3,
    p,
    SuperBit.enMotors.M4,
    n
    )
}
radio.onReceivedNumber(function (receivedNumber) {
    if (receivedNumber == 1) {
        basic.showArrow(ArrowNames.North)
        F()
    } else if (receivedNumber == 2) {
        basic.showArrow(ArrowNames.South)
        B()
    } else if (receivedNumber == 3) {
        basic.showArrow(ArrowNames.West)
        L()
    } else if (receivedNumber == 4) {
        basic.showArrow(ArrowNames.East)
        R()
    } else if (receivedNumber == 5) {
        stop()
        SuperBit.RGB_Program().showColor(neopixel.colors(NeoPixelColors.Indigo))
        SuperBit.RGB_Program().show()
    } else if (receivedNumber == 6) {
        turnleft()
    } else if (receivedNumber == 7) {
        turnright()
    } else {
        basic.showIcon(IconNames.Angry)
    }
})
function F () {
    SuperBit.MotorRunDual(
    SuperBit.enMotors.M1,
    p,
    SuperBit.enMotors.M2,
    p
    )
    SuperBit.MotorRunDual(
    SuperBit.enMotors.M3,
    p,
    SuperBit.enMotors.M4,
    p
    )
}
function turnright () {
    SuperBit.MotorRunDual(
    SuperBit.enMotors.M1,
    90,
    SuperBit.enMotors.M2,
    90
    )
    SuperBit.MotorRunDual(
    SuperBit.enMotors.M3,
    70,
    SuperBit.enMotors.M4,
    70
    )
}
function stop () {
    SuperBit.MotorRunDual(
    SuperBit.enMotors.M1,
    0,
    SuperBit.enMotors.M2,
    0
    )
    SuperBit.MotorRunDual(
    SuperBit.enMotors.M3,
    0,
    SuperBit.enMotors.M4,
    0
    )
}
input.onButtonPressed(Button.A, function () {
    turnleft()
    basic.showLeds(`
        # # # . .
        # # . . .
        # . # . .
        . . . # .
        . . . . #
        `)
})
input.onGesture(Gesture.LogoUp, function () {
    radio.sendNumber(2)
    basic.showArrow(ArrowNames.South)
})
input.onGesture(Gesture.TiltLeft, function () {
    radio.sendNumber(3)
    basic.showArrow(ArrowNames.West)
})
function B () {
    SuperBit.MotorRunDual(
    SuperBit.enMotors.M1,
    n,
    SuperBit.enMotors.M2,
    n
    )
    SuperBit.MotorRunDual(
    SuperBit.enMotors.M3,
    n,
    SuperBit.enMotors.M4,
    n
    )
}
input.onGesture(Gesture.ScreenDown, function () {
    radio.sendNumber(5)
})
input.onButtonPressed(Button.AB, function () {
    radio.sendNumber(5)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . # . .
        . . . . .
        . . . . .
        `)
})
input.onButtonPressed(Button.B, function () {
    turnright()
    basic.showLeds(`
        . . # # #
        . . . # #
        . . # . #
        . # . . .
        # . . . .
        `)
})
function R () {
    SuperBit.MotorRunDual(
    SuperBit.enMotors.M1,
    p,
    SuperBit.enMotors.M2,
    n
    )
    SuperBit.MotorRunDual(
    SuperBit.enMotors.M3,
    n,
    SuperBit.enMotors.M4,
    p
    )
}
input.onGesture(Gesture.TiltRight, function () {
    radio.sendNumber(4)
    basic.showArrow(ArrowNames.East)
})
input.onGesture(Gesture.LogoDown, function () {
    radio.sendNumber(1)
    basic.showArrow(ArrowNames.North)
})
function turnleft () {
    SuperBit.MotorRunDual(
    SuperBit.enMotors.M1,
    70,
    SuperBit.enMotors.M2,
    70
    )
    SuperBit.MotorRunDual(
    SuperBit.enMotors.M3,
    90,
    SuperBit.enMotors.M4,
    90
    )
}
let n = 0
let p = 0
basic.showIcon(IconNames.Angry)
radio.setGroup(121)
p = 150
n = -150
SuperBit.RGB_Program().setBrightness(120)
basic.forever(function () {
	
})
