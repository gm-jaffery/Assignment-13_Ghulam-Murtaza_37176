
1. Audit Table
| Claim in AI Interpretation | Colour | How Checked | Accepted / Rejected |
| "Staple A prices increased by 19.31% over the quarter." | Green | Recomputed via pandas (`(120.5 - 101) / 101 * 100`) | Accepted |
| "Prices rose due to supply chain disruptions and transport costs." | Red | Checked data columns (no supply chain or transport metrics present) | Rejected |
| "The median is more robust to extreme values than the mean." | Amber | Verified mathematically via outlier stress-testing | Accepted (Explanation) |

2. Classmate Transcript Excerpt
Classmate: "If the mean is the mathematical average, why isn't it always the typical price?"  
Analyst: "Because extreme highs or lows pull the mean away from where most data points cluster. The median finds the exact middle value, representing the typical consumer experience when data is skewed."  
Classmate: "Got it, so the median prevents extreme spikes from distorting reality."  
Analyst: "Exactly."

3. Reflection
The initial draft overreached by attributing price increases to external supply chain and transport factors. Because the teaching dataset only records dates, cities, and prices without contextual economic drivers, the causal claim ("transport fuel hikes forced retailers to raise prices") violated the descriptive limits of the data.
