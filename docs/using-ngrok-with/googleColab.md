---
title: Google Colab
---

# Using ngrok with Google Colab

If you're looking to run the ngrok agent into your Google Colab project, you can leverage the [pyngrok project](https://pyngrok.readthedocs.io/en/latest/integrations.html#google-colaboratory) to start a tunnel in your project.
import matplotlib.pyplot as plt
import pandas as pd

# 数据
data = {
    '日期': ['2025-02-27', '2025-02-28', '2025-03-03', '2025-03-05', '2025-03-06'],
    '市场行情描述': [
        '外盘坚挺支撑现货市场行情，加上到货有限，提振持货商心态。',
        '外盘坚挺支撑现货市场行情，加上到货有限，提振持货商心态。',
        '外盘坚挺支撑现货市场行情，加上到货有限，提振持货商心态。',
        '外盘坚挺支撑现货市场行情，加上到货有限，提振持货商心态。',
        '外盘坚挺支撑现货市场行情，加上到货有限，提振持货商心态。'
    ]
}

# 创建走势图
plt.figure(figsize=(10, 6))
plt.plot(data['日期'], [1] * len(data['日期']), 'o-', markersize=8)
plt.title('广州港鱼粉市场行情走势')
plt.xlabel('日期')
plt.ylabel('市场行情')
plt.yticks([1], ['外盘坚挺支撑现货市场行情，加上到货有限，提振持货商心态。'])
plt.grid(True)
plt.show()
