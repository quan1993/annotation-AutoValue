import com.google.auto.value.AutoValue;

@AutoValue
public abstract class Complex {

	public static Complex createFromCartesian(double real, double imaginary) {
        return new AutoValue_Complex(real, imaginary);
    }
 
    public static Complex createFromPolar(double r, double theta) {
        return new AutoValue_Complex(r * Math.cos(theta), r * Math.sin(theta));
    }
 
    public abstract double getReal();
    public abstract double getImaginary();
}
