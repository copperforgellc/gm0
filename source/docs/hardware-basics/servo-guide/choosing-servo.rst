Choosing a Servo
================

For many applications, you can just use one of the three common :term:`servos <Servo>` in FTC, `REV Smart Servo <https://www.revrobotics.com/rev-41-1097/>`_ or `goBILDA Dual Mode Servo (Torque) <https://www.gobilda.com/2000-series-dual-mode-servo-25-2/>`_, or `goBILDA Dual Mode Servo (Speed) <https://www.gobilda.com/2000-series-dual-mode-servo-25-3-speed/>`_ However, sometimes these :term:`servos <Servo>` are not enough. Here are some important :term:`servo <Servo>` features to consider when selecting a :term:`servo <Servo>`.

Servo Type: Regular or Continuous
---------------------------------

:term:`Servos <Servo>` which can rotate to a given position based on PWM input signal are called **regular servos**. In addition, there are also **continuous rotation servos**, which are effectively just small motors in a :term:`servo <Servo>` form factor. They have no position control; instead, PWM signal is used to control their rotation speed.

Both REV Smart Servo and goBILDA Dual Mode servos (which are both based on FR5311m programmable servo by Feetech) can be used as either regular or continuous rotation servos. To switch between these two modes, you need to use a :term:`servo programmer <SRS Programmer>`, available separately from REV or goBILDA.

.. warning:: Some vendors offer continuous rotation *option* on some :term:`servos <Servo>`. These options are modifications to the original :term:`servo <Servo>` made by the vendor and are illegal in FTC. The only legal continuous rotation servos are CR servos direct from the **manufacturer/factory**. If you have a seller modify a :term:`servo <Servo>` for continuous rotation, that :term:`servo <Servo>` is not legal.

Servo Torque And Speed
----------------------

:term:`Servo` output power is measured in both **speed** and **torque**. Speed (normally in seconds per 60°) refers to how fast the :term:`servo <Servo>` turns 60 degrees in Standard Rotation mode. Torque (usually measured in oz-in or in kg-cm) refers to the amount of force the :term:`servo <Servo>` can apply to a lever.

For reference, if you put a 1” bar on a servo, then put a force gauge on the end, the torque rating of the servo (in oz-in) will be measured. As you may know, speed and torque have an inverse relationship. Generally you can find some insanely powerful servos that are pretty slow (slower than 0.20 s/60°) or some less powerful ones with faster ratios (anything faster than 0.12 s/60° is considered very fast).

Finding the right :term:`servo <Servo>` for your application can be tough, but a good way is trying to decide if you need more speed or torque, and if your :term:`servo <Servo>` will experience shock loads or not.

Durability and Servo Gear Material
----------------------------------

The two things that threaten a :term:`servo’s <Servo>` longevity are the internal motor burning out and more commonly, the :term:`gears <Gear>` stripping inside the :term:`servo <Servo>`. A motor burning out is pretty uncommon, but it can happen under large loads for a prolonged amount of time.

.. caution:: You should **never** stall a servo against an immovable object.

Gear stripping is a very common problem which occurs when the torque needed to actuate a component exceeds that of the :term:`servo's <Servo>` maximum torque. There are two main cases when this can occur.

- Shock load from external force can strip the :term:`gears <Gear>` easily, regardless of which material the :term:`gears <Gear>` are made from. An example could be the component slamming into the field wall or another robot.
- Shock load from reversing directions on an object that is too heavy can strip the :term:`gears <Gear>`. Torque increases with mass and also distance from the center of rotation. If the component being actuated is far from the :term:`servo <Servo>`, the long lever arm means larger torque. Furthermore, if the component is moving, reversing direction also will require more torque. Thus, the principle is that components should be light and not reverse direction suddenly to prolong :term:`servo <Servo>` life.

Shock load resistance is impacted directly by the material the :term:`gears <Gear>` are made from. This ranges from plastic to titanium, so let’s go down the list, starting from the weakest.

- **Plastic**: with low power :term:`servos <Servo>`, these are normally okay. Generally used for applications in model airplanes such as ailerons. FTC applications include light load mechanisms which will not have direct contact with any game elements or the field. An example could be a servo which opens a trapdoor or moves game elements within the robot.
- **Karbonite**: Hitec’s :term:`gear <Gear>` plastic is a very durable and long lasting plastic and is very good under long use and low load. Be aware that it can strip easily under the shock loads found in FTC. Karbonite is more durable than plastic but still suffers from shock loads.
- **Brass**: Brass :term:`gears <Gear>` are stronger than plastic but also suffer greatly when faced with shock loads in FTC like intake wrists and deposit buckets. It’s found on slightly higher end servos such as the REV Smart Servo.
- **Steel**: This is where we start getting big. Steel :term:`gears <Gear>` are very durable and you’ll have a tough time stripping these. In general, expect to pay a premium. The goBILDA Dual mode servos (v2) is an example of steel :term:`gear <Gear>` :term:`servo <Servo>`.
- **Titanium**: Titanium is where you get into really high end, virtually unbreakable :term:`servos <Servo>`. Starting from $75, they can reach over $150.

Servo Size
----------

:term:`Servos <Servo>` come in different sizes. Fortunately, almost all manufacturers use the same standard set of :term:`servo <Servo>` sizes, ranging from sub-micro to large. The two sizes commonly used in FTC are *standard size* (which includes REV Smart Servo and goBILDA Dual Mode Servos) and *large size* (also known as quarter-scale) :term:`servos <Servo>`. However, large :term:`servos <Servo>` are quite uncommon.

Note that while in general, the larger the size, the more powerful the :term:`servo <Servo>`, it is not a strict rule. You can buy very powerful standard size :term:`servos <Servo>` - just expect to pay more for them.

Servo Spline
------------

The output shaft of the :term:`servo <Servo>` is commonly called the **spline**. Most servos have industry standard 25 tooth spline (also known as F3); in particular, this is the spline used by REV Smart Servo and goBILDA Dual Mode servos. However, Hitec servos using 24 tooth spline are also very popular.

.. attention:: Please check the spline type before you buy the :term:`servo <Servo>` - otherwise, your :term:`servo <Servo>` attachments will not fit.

For more info about servo splines, please check https://www.servocity.com/servo-spline-info/.

Cost
----

:term:`Servos <Servo>` range from cheap $7 :term:`servos <Servo>` for light applications, all the way up to some Hitec or Savox :term:`servos <Servo>` for close to $200.

By far the best bang for your buck :term:`servos <Servo>` out there are the Feetech dual mode :term:`servos <Servo>`, which is a programmable type of :term:`servo <Servo>`. This includes both the **REV SRS** (Smart Robot Servo) and **goBILDA Dual Mode servos**.

The biggest downside to the REV SRS and the old goBILDA servos (25-1) are their brass :term:`gears <Gear>`. Coupled with high output power, this meant that stripping :term:`gears <Gear>` with any shock load was commonplace. The new goBILDA Dual Mode servos (25-2) and (25-3) have steel :term:`gears <Gear>`, but are new and aren’t as competition tested as other servos.

The next big name in FTC :term:`Servos <Servo>` is Hitec, who are a huge name in hobby :term:`servos <Servo>` for decades and are very well trusted. Their low end :term:`servos <Servo>` are inexpensive but easily broken.

A mid-priced Hitec :term:`servo <Servo>` is the HS 485-HB/488-HB servo, with Karbonite :term:`gears <Gear>`. While it shouldn’t be used in high load applications, it is fine for general use such as claws or trapdoors. 485HB uses 24 tooth spline; 488 HB uses 25 tooth spline (recommended).

Where Hitec really shines is the high end market. If your budget is over $100, you can get into some very powerful Hitec :term:`servos <Servo>`. Most have titanium :term:`gears <Gear>` and are programmable, so you can dial in the performance and range to exactly what you need.

The last big player in the :term:`servo <Servo>` market in FTC is Savox, which produces great mid-high range :term:`servos <Servo>` (think $60-$100+). They are made with titanium :term:`gears <Gear>` (close to bulletproof) and are **fast**. Savox :term:`servos <Servo>` are mostly brushless and coreless, so they do tend to scream a little under load, but they’re definitely worth it if your budget allows for it.

Best Value
----------

- Low Priced (~$18)
   - HiTec 488HB
   - Futaba servos
- Medium Priced (~$25)
   - `goBILDA Dual Mode Servo (Torque) (25-2) <https://www.gobilda.com/2000-series-dual-mode-servo-25-2/>`_
   - `goBILDA Dual Mode Servo (Speed) (25-3) <https://www.gobilda.com/2000-series-dual-mode-servo-25-3-speed/>`_
   - `REV Smart Servo <https://www.revrobotics.com/rev-41-1097/>`_
   - `25kg Coreless Servo <https://longrobotics.com/product/25kg-coreless-servo-ds3225sg/>`_
- Best Performance ($75+)
   - Savox titanium servos
   - Hitec titanium servos

REV and goBILDA :term:`servos <Servo>` can be purchased from REV and goBILDA websites respectively. For all other servos some good sources are `ServoCity <https://www.servocity.com/>`_ or `Amazon <https://www.amazon.com/>`_.
