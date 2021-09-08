# SetandHasSet

When overriding the equals() method in the HeavenlyBody class, it was made sure
that it would not return true if a HeavenlyBody was compared to a subclass of itself.

That's done to demonstrate that method, but it was actually unnecessary in
the Heavenly Body class.

Why is that unnecessary?

Answer:

The HeavenlyBody class is declared final, so it cannot be subclassed.
The Java String class is also final, which is why it can safely use the
instanceof method without having to worry about comparison with a subclass.

