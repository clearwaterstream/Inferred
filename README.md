# Inferred
Assign value to a string based on the string variable's name. This is a util for the truly lazy ones - which means pretty much everyone.

### Examples

Instead of doing this  

```
public class OrderStatus
{
  public static readonly string Created = nameof(Created);
  public static readonly string SentToFulfillmentCentre = nameof(SentToFulfillmentCentre);
  public static readonly string Shipped = nameof(Shipped);
}
```

You can do this

```
public class OrderStatus
{
  public static readonly string Created = new Inferred();
  public static readonly string SentToFulfillmentCentre = new Inferred();
  public static readonly string Shipped = new Inferred();
}
```
