#Making Chicken tikka Masala

##Step by Step Human process
Start
Marinade
    Combine Dahi Yoghurt, spices and Gigi paste, add chopped chicken
    Refridgerate for at least 2 hours, preferably overnight.
Make the Makhani Gravy
    Dry Roast Spices
    Add oil
    Chop and fry one onion
    chop and fry 2-12 birds eye chilis
    Add 1 16oz can of whole tomatoes, crushing them by hand as you add them
    Scrape the fond off of the pan with a wooden spoon after introducing the tomato liquid
    Blend to a smooth consistency with an immersion blender
    add 1 pint cream
    add 2 tbs kasuri methi
    add 4 tbs salt
    add 2 tbs sugar
    add 1 tbs garam masala
    mix to combine
    cook on low until gently bubbling and thickened

Roast the Chicken
    Remove chicken from marinade, shaking off excess
    Broil in a tandoori, if available, or oven, otherwise for 10 minutes, or until almost cooked to 165 degrees int


Combine
    Add chicken to the gravy, and finish cooking until the largest piece of chicken reaches 165 deg int
    Serve with rice.
End

_Notes: Chop and fry instruction is re-used a lot.  Probably would make for a good function.
Roast instruction means two different things in different contexts.  Make sure to differentiate between them if defining them as functions.
Spices should be defined as an array, to reduce repeating
Mix instruction is a basic one that can be repeated as a function
Broiling the chicken should be represented by an if else statement regarding the availability of a tandoor oven
_

##Diagram
Chicken Tikka Masala
    Ingredient (?)
    Gigi Paste (object used in marinade and Makhani Gravy)
    chop (function to be used later)
    fry (function to be used later)
    add (function to be used later)
    spices (array to be used later)
    Tandoori Chicken (object)
        Chicken Prep (function)
        Marinade (object)
                Gigi Paste (instance)
    Makhani Gravy (object)
        Pan
        Add Spices (array)
        Gigi Paste (instance)
        add oil
        chop (function) onion
        chop (function) chilis
        fry (function) onion
        fry (function) chilis
        add tomatoes (for loop to crush them)
        add tomato juice
        mix, scraping the bottom of the pan
        add 1 pint cream
        add 2 tbs kasuri methi
        add 4 tbs salt
        add 2 tbs sugar
        add 1 tbs garam masala
        mix until combined
    Roast Chicken
        Remove chicken from marinade (while loop until bowl is empty)
        shake chicken (while marinade is falling off)
        If tandoor is available
            Skewer chicken
            Add to tandoor
            cook until 160F
            remove from oven
        else
            add chicken to sheet pan
            broil until 160F
            remove from oven
    Combine
        Add chicken to gravy
        Stir
        Cook on low until chicken reaches 165F
    Serve
        ladle chicken tikka masala to plate



##Pseudocode

Chicken Tikka Masala
Start: Start the Program

Init
    Mix ()
        WHILE contents NOT Homogenous stir contents

    Gigi Paste (object used in marinade and Makhani Gravy)
        grind 3 oz ginger
        grind 3 oz garlic
        mix ()

    chop (function to be used later)
        WHILE ingredient size > 1cm, /2

    fry(ingredient) (function to be used later)
        Add 1 tbs oil to pan
        Add ingredient to pan
        cook, stirring constantly, until softened

    add (function to be used later)
    
    ARRAY spices = [4tsp turmeric, 4 tsp coriander, 4 tsp cumin, 2 tbs garam masala, 8 pods ground cardamom, 2 tbs ground black pepper, 3 tbs kashmiri pepper]
    Class Cookware
        pan = 
        size: 9.5 inch 
        type: skillet

        pot = 
        size 2 quart 
        type: saucepan
    Class 
        oven = 

    tandoor = 
OBJECT Tandoori Chicken
        FUNCTION Chicken Prep
            while chicken size > 1 inch, /2
            This = chicken piece

        FUNCTION Make Marinade
            Gigi Paste (instance)
            2 lb dahi yoghurt
            add spices
            mix ()
            add chicken Prep to marinade
            If restTime < 2hrs, rest
            ELSE proceed to roast chicken
        
        FUNCTION Roast Chicken
            Remove chicken from marinade
                While Chicken remains, -1 chicken piece from bowl
                IF marinade is falling off, shake chicken
                ELSE proceed
            
            If tandoor is available
                Skewer chicken
                    Kebab = push metal skewer through chicken
                Add to tandoor
                    Insert kebab into tandoor opening, pointed side down
                cook until 160F
                remove from oven
            else
                add chicken piece to sheet pan
                broil until 160F
                remove from oven

OBJECT Makhani Gravy
        Pan
        Add Spices
        While no smoke, Shake Pan             
        Add Gigi Paste 
        Mix ()
        chop (onion)
        chop (chilis)
        fry (onion)
        fry (chilis) 
        add tomatoes
            While tomatoes in can > 0, remove 1 tomato, crush in hand, add to pan
        add tomato juice
        mix, scraping the bottom of the pan
        add 1 pint cream
        add 2 tbs kasuri methi
        add 4 tbs salt
        add 2 tbs sugar
        add 1 tbs garam masala
        mix ()

Combine
        Add chicken to gravy
        Mix ()
        Cook on low until chicken reaches 165F
    Serve
        ladle chicken tikka masala to plate
END