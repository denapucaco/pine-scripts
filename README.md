# pine-scripts

## ema-cluster-psar-breakout.pine

Setting alert in TradingView (step by step)

1. Add the updated script to chart, click the alarm clock icon → Create Alert.
2. In the Condition dropdown, pick indicator name (e.g., "EMA Cluster PSAR Breakout").
3. In the second dropdown, select "Any alert() function call" — this is the only option needed since script controls everything with alert().
4. Leave the Message field as default (the {{default}} placeholder, or just leave it — whatever text you put in alert() in Pine is what gets sent, the Message box is ignored/overridden for this condition type in most setups — but to be safe, TradingView shows a note that the script's own message is used).
5. Set Expiration (or "Open-ended" if you have that plan tier).
6. Under Notifications, enable Webhook URL and paste your webhook endpoint URL (https://api.telegram.org/bot<TOKEN>/sendMessage)
7. Click Create.
