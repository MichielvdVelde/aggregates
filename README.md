Months worth of ore and mineral aggragated market statistics for Eve Online.

The model for convenience:

```typescript
export class Aggregate {
  @prop({ required: true, immutable: true })
  public readonly type!: "buy" | "sell";

  @prop({ required: true, immutable: true })
  public readonly typeId!: number;

  @prop({ required: true, immutable: true })
  public readonly locationId!: number;

  @prop({ required: true, immutable: true })
  public readonly weightedAverage!: number;

  @prop({ required: true, immutable: true })
  public readonly median!: number;

  @prop({ required: true, immutable: true })
  public readonly stddev!: number;

  @prop({ required: true, immutable: true })
  public readonly volume!: number;

  @prop({ required: true, immutable: true })
  public readonly orderCount!: number;

  @prop({ required: true, immutable: true })
  public readonly percentile!: number;

  @prop({ required: true, immutable: true, default: Date.now })
  public readonly retrievedOn!: Date;
}
```
